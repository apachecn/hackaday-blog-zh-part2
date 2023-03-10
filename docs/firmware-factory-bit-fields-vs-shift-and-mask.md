# 固件工厂:位域与移位和屏蔽

> 原文：<https://hackaday.com/2015/08/28/firmware-factory-bit-fields-vs-shift-and-mask/>

使用嵌入式系统通常包括编写与硬件接口的代码。这通常意味着在寄存器级别上工作。不管我们谈论的是 UART、模数转换器、LCD 控制器还是其他小发明。迟早，你将不得不打开数据手册，弄清楚如何与外部设备对话。要在这方面取得成功，你必须成为钻头操纵大师。

硬件设计者不喜欢浪费空间，所以模式、设置和其他小块信息通常以打包位的形式存储。我们的处理器通常一次访问一个字节(或一个字)，那么最好的处理方式是什么呢？就像软件工程中的许多其他主题一样，有多种方法来剥这只猫的皮。在 C 语言(及其衍生语言)中有两个主要选项:移位和掩码，以及位域。

[![ad-pll-ctrl](img/2183926271aa3ce3720da7e13e115dcc.png)](https://hackaday.com/wp-content/uploads/2015/08/ad-pll-ctrl.png)

考虑 ADI 公司的模数转换器(ADC)adau 1977 的寄存器。这里发生了很多事情。我们有 6 个独立的数据元素要处理。位 7 是只读位，而其余位是读/写位。3 个最低有效位作为单个 3 位值处理，用于选择 ADC 的主时钟。

### 位字段

c 语言描述按位数据的原生接口是位字段。位域的定义就像结构一样，这意味着它们非常易于阅读代码。位域的缺点是不可移植。使用位域意味着非常信任你的编译器会按照你的期望去做。

在位域中，我们将 PLL 控制寄存器描述如下:

```

struct 
{
 unsigned char clockSelect:3;
 unsigned char res2 :1;
 unsigned char clkSource :1;
 unsigned char res1 :1;
 unsigned char pllMute :1;
 unsigned char pllLock :1;
} PllControlRegister;

```

访问位域就像一个结构:

```

struct PllControlRegister myRegister;
myRegister.pllMute = 0;

```

简单对吗？细节决定成败。位字段是不可移植代码的缺陷之一。[连 Linux 内核黑客都被咬过](https://lwn.net/Articles/478657/)。如果您正在从事的项目是特定于架构(和编译器)的，并且您知道编译器将如何工作，那么您就成功了！但是，如果您将来计划在不同的系统上重用这些代码，您就是在自找麻烦。原因如下:C 标准没有定义位字段应该如何排序。事实上，它说:[“一个单元内位字段的分配顺序(高阶到低阶或低阶到高阶)是实现定义的。”](http://c0x.coding-guidelines.com/6.7.2.1.html)

据此，我们无法知道 pllLock 是会像我们预期的那样位于最高有效位，还是最低有效位。当您在 32 或 64 位机器上添加更大的位字段、字节序以及跨越存储边界的字段填充时，事情会变得更加复杂。如果你对可移植代码感兴趣，你最好使用另一种方法，shift 和 mask，我将在下面介绍。现在，让我们来讨论一个真实的例子，其中位域是更好的选择。

Microchip 的 PIC 系列处理器在它们自己的包含文件中广泛使用位域。例如， [PIC16F1829](http://www.microchip.com/wwwproducts/Devices.aspx?product=PIC16F1829) 微控制器上的 INTCON(中断控制)寄存器定义如下:

```

struct 
{
   unsigned IOCIF :1;
   unsigned INTF :1;
   unsigned TMR0IF :1;
   unsigned IOCIE :1;
   unsigned INTE :1;
   unsigned TMR0IE :1;
   unsigned PEIE :1;
   unsigned GIE :1;
}INTCONbits_t;

```

(实际。h 文件有一个联合，但是我在这里把事情简化了一点)

Microchip 可以在这里使用位域，因为他们知道编译器会做什么——是他们写的！INTCON 也是 PIC 本身的内部寄存器，所以不用担心编写可移植代码。额外的好处是，PIC 具有位设置和清除操作码，可以在其所有 RAM 上操作。编译器足够聪明，可以将任何位域操作翻译成适当的 bsf 和 bcf 操作码，它们在单个周期内运行。

### 移位和屏蔽

像这样处理操作的更安全的方法是移位和屏蔽。顾名思义，它使用一个移位操作来建立一个掩码，然后我们使用该掩码和一个逻辑运算符来设置或清除一个特定的位。我们不想在实际的硬件上执行所有这些工作，所以最好的办法是使用 RAM 中寄存器的影子。首先将硬件寄存器读入 RAM，然后对 RAM 映像进行修改，最后将 RAM 映像写回硬件寄存器。这就是“读-修改-写”这个术语的由来。我知道这听起来很复杂，但是在使用几次之后，用阴影寄存器进行移动和蒙版就变成了第二天性。

回头看看本文顶部的 ADC 寄存器，假设我们要设置 pllMute，即位 6。逻辑“或”运算可用于设置一个位。在这种情况下，你需要用 1 来屏蔽你想要改变的所有位。

为简单起见，假设这些例子中的 PllControlRegister 是一个内存映射的 I/O 位置，称为“pllCtlReg”。

```

unsigned char pllShadow;
unsigned char mask = 1;
pllShadow = pllCtlReg;     //Read the current value of pllCtlReg
//now build the mask
mask = mask &lt;&lt; 6;          //Shift to get 0x40, or b0100 0000
pllShadow | = mask;         //Logical OR will SET the only bit 6 in our shadow
pllCtlReg = pllShadow;     //write the shadow back to the hardware

```

如果我们要清除某个位，逻辑 AND 是可行的方法，但这一次您需要用 0 来屏蔽您要更改的位，所有其他位将被设置为 1。

```

unsigned char pllShadow;
unsigned char mask = 1;
pllShadow = pllCtlReg;      //Read the current value of pllCtlReg
//now build the mask
mask = mask &lt;&lt; 6;           //Shift to get 0x40, or b0100 0000 
mask = ~mask;               //logical NOT gives us 0xBF, or b1011 1111 
pllCtrlReg &amp;= mask;         //Logical AND will clear only bit 6 in our shadow.
pllCtlReg = pllShadow;      //write the shadow back to the hardware

```

如果你需要切换位，逻辑异或(异或，或^运算符)是首选工具。我只是展示了一个最基本的方法来执行移位和遮罩。有很多方法可以执行相同的操作。您可以使用#defines 或预处理宏，甚至函数来执行这些相同的任务。这完全取决于对您的应用程序最重要的是什么:内存空间，还是执行速度。