# 学习用于 FPGAs 的 Verilog:工具和构建加法器

> 原文：<https://hackaday.com/2015/08/19/learning-verilog-on-a-25-fpga-part-i/>

在过去的一年里，我们有几篇关于晶格半导体[冰棍](http://www.latticesemi.com/icestick)的帖子[，如下所示。该板看起来像一个没有外壳的杂草丛生的 u 盘，但它实际上是一个 FPGA 开发板。规格适中，I/O 数量有限，但价格(大约 22 美元，取决于你在哪里购物)是正确的。我一直想做一个 Verilog 视频系列，并决定这将是正确的目标平台。你可以在不倾家荡产的情况下用真正的 FPGA 做实验。](http://hackaday.com/2015/05/29/an-open-source-toolchain-for-ice40-fpgas/)

实际上，你可以不用真正的硬件就能学到很多关于 FPGAs 的知识。正如您将看到的，许多 FPGA 开发都是在 PC 上运行的模拟 FPGA 上进行的。但如果你像我一样，闪烁虚拟 LED 并不像让真实的 LED 发光那么令人兴奋。然而，对于我提到的前两个例子，除了计算机之外，你不需要任何硬件。如果你想做好准备，你可以订购一个冰棍，也许它会在本系列第三部分出版之前到达。

我不会直接尝试教 Verilog。如果你知道 C，你可以很快学会，如果你不知道，有大量的基于文本和基于视频的教程可供选择(我会在这篇文章的末尾添加一些)。不过，我将指出一些会让新 FPGA 设计人员出错的关键领域，通过遵循示例代码，您将很快上手。

# 选择 Verilog 模拟器

![EDA Playground Screenshot](img/a51827615172555181425693601085c3.png)

EDA Playground Simulates Verilog in the Browser

对于第一部分，您需要一个 Verilog 模拟器。我将使用 [EDAPlayground](http://edaplayground.com) ，因为它是免费的，可以在你的浏览器中运行。不需要安装软件，也不用担心你使用什么疯狂的操作系统(比如 Windows)。如果你有一个现代化的浏览器，你就万事俱备了。

我知道有些人不想在网上工作，或者不想创建一个帐户(老实说，这只是教程代码，创建一个一次性电子邮件地址很容易)。如果你实在无法忍受，你可以用 [Icarus Verilog](http://iverilog.icarus.com/) 运行你桌面上的所有例子(用 [GTKWave](http://gtkwave.sourceforge.net/) 显示结果)。我只是不会谈论如何做到这一点。如果你想走那条路，你可以阅读伊卡洛斯[号的介绍](http://iverilog.wikia.com/wiki/Getting_Started)。我还是建议你坚持用 EDAPlayground 做教程。

对于第三部分中使用的 FPGA 工具，我使用的是[开源 Icestorm 工具](http://hackaday.com/2015/07/28/open-source-fpga-toolchain-builds-cpu/)。我试着使用 Lattice 工具，但是安装和许可它们是令人心碎的困难。我将在第三部分对此进行更多的阐述。

# 关于目标硬件

冰棍上有一个普通的 FPGA。从其手册来看，它具有以下特点:

*   高性能、低功耗 iCE40HX1K FPGA
*   FTDI 2232H USB 设备允许 ice 设备编程和与 PC 的 UART 接口
*   Vishay TFDU4101 IrDA 收发器
*   五个用户指示灯(一个绿色，四个红色)
*   2 x 6 位置勤奋 Pmod 兼容连接器支持许多其他外设连接
*   识别 12Mhz MEMS 振荡器
*   微米 32Mbit N25Q32 SPI 闪存
*   0.1 英寸通孔连接上的 16 个 LVCMOS/LVTTL (3.3V)数字 I/O 连接

FPGA 不是很大，但它足够容纳一个简单的 CPU ( [我们之前已经讨论过 CPU 了](http://hackaday.com/2015/07/28/open-source-fpga-toolchain-builds-cpu/))。不过，我们不会从 CPU 开始。我们将从更简单的开始。

# 让我们建造一个加法器

在任何 FPGA 上构建的电路主要有两种:组合电路和时序电路。区别很简单:组合逻辑就是所有的逻辑门。电路的过去状态并不重要。给定一组特定的输入，输出将是相同的。时序电路(几乎总是有一个触发器)有一些改变输出的先前状态的记忆。我想展示两者的例子，以及如何将它们映射到板上。

我们将构建的示例电路有三个主要部分。第一个是两位加法器电路，显示二进制和，并在电路板的五个 led 中的两个上进位。这是一个简单的组合电路。它不使用板载 12MHz 时钟。另外两部分会。第一个时序电路将是一个简单的存储器，如果加法器产生了进位(当然是在复位之后)，它就锁存 true。另一个时序电路是一组计数器，它们组合起来提供来自 12MHz 时钟的 1/2 秒脉冲。

## Verilog 与原理图条目

对于简单的电路，很容易画出如上图所示的原理图，然后机器将其翻译到 FPGA，或者手动翻译到 Verilog。一些工具支持这一点，您可能认为这是正确的做法。我知道我开始的时候是这样的。

事实是，当你远离简单的事物后，这些图表会非常痛苦。例如，考虑一个七段解码器。如果你花几分钟的时间，你也许能算出执行该功能所需的“与”或“与非”门(也就是说，将 4 位二进制数转换成 7 段显示)。但是需要几分钟。

如果你使用 Verilog，你可以采取一个简单的方法，只要写出你想要的门。这是可行的，但通常不是正确的答案。相反，您应该描述您想要的电路行为，Verilog 编译器将推断出创建您需要的电路。对于七段解码器，这可以简单到:

```
always @(*)
case (number)
 4'h0: dispoutput <= 7'b1111110;
 4'h1: dispoutput <= 7'b0110000;
 4'h2: dispoutput <= 7'b1101101;
. . .
```

我承诺我会指出 Verilog 的一些奇怪之处，所以让我们更详细地看一下。`always`语句告诉 Verilog，只要您在其中使用的任何输入发生变化，就应该执行下面的代码。由于没有时钟，这就推断出一个组合电路。`case`语句类似于 c 语言中的`switch`语句。有趣的数字是 4 位十六进制(4'h1)和 7 位二进制(7'b1101101)。因此，代码指示 FPGA(或者更准确地说，Verilog 编译器)检查数字，并根据输入设置`dispoutput`。

顺便说一下，`<=`字符是一个非阻塞赋值。您还可以在这里使用等号来创建一个阻塞赋值。目前，这种差异并不重要，但是当我们使用顺序设计时，我们将再次讨论这个主题。

从这个你想要的描述中，Verilog 编译器将推断出正确的门，甚至可以执行一些优化。FPGA 和在微控制器上构建东西的关键区别在于并行性。如果你在一个 Arduino 上写类似的 C 代码，那么它的每一个副本都需要一些执行时间。例如，如果你有 50 个解码器，CPU 必须依次为每个解码器服务。在 FPGA 上，你只能得到 50 个相同电路的副本，所有副本都同时运行。

# Verilog 的要点 1: Verilog 是不可执行的(除非它是可执行的)

这是非常重要的一点。有了 FPGA，驱动每个显示器的电路就可以一直工作。当然，通过门会有小的延迟(可能是皮秒)，但即使是分立电路也是如此。这并不是因为 FPGA 正在执行 Verilog 代码行或一些等效的结构。Verilog 成为连接电路元件的连接线，就好像你在 PCB 上有一大堆门，你用绕线把它们连接起来。

这有一个例外。在仿真过程中，Verilog 确实像一种编程语言，但它有非常具体的规则来保持时序与 FPGA 上的相同。但是，它也允许您编写不可转移到 FPGA 的结构。比如一个子程序调用在硬件上没有意义，但是你可以在仿真的时候做。一般来说，您希望避免不可合成的 Verilog，除非在编写您的测试平台(您的仿真的驱动程序；我一会儿再详细讲)。

回头看看加法器原理图。求和是一个简单的`XOR`门，进位是一个`AND`门。如果我愿意，我可以用 Verilog 来表达，就像这样:

```
assign carry=inA&inB;
assign sum=inA^inB;
```

不过，让 Verilog 来解决这个问题更明智。我可以像这样创建一个包含两位的变量:

```
reg [1:0] fullsum;
```

然后我可以说:

```
assign fullsum={1’b0, inA} + {1’b0, inB};
assign carry=fullsum[1];
assign sum=fullsum[0];
```

拉条将一位线`inA`和`inB`变成两位量。在这个简单的例子中，我可能实际上坚持使用第一种方法，但是如果你回想一下 7 段解码器，你会发现尽可能使用这种推断方式是有意义的。

# 模块和定义

当你看下面的视频或者浏览代码时，你会注意到我忽略了一些小细节。首先，所有这些代码都存在于一个模块中。你可以把一个模块松散地看作一个子程序，或者更好的是一个 C++类。其他模块可以创建模块的副本，并将不同的信号映射到其输入和输出。还有所有使用的网络的定义(我们已经讨论过连线和规则):

```
module demo(
 output LED1,
 output LED2,
 output LED3,
 output LED4,
 output LED5,
 input PMOD1, // input A
 input PMOD2, // input B
 input PMOD3, // run/stop
 input PMOD4 // reset
 );

// Alias inputs
 wire inA;
 wire inB;
 assign inA=PMOD1;
 assign inB=PMOD2;

```

请注意，我希望信号有与物理硬件相关的名称(如`LED1`和`PMOD2`，但后来我想使用更有意义的名称，如`inB`。`assign`语句建立了这种联系。这是该语句的一个简单应用。如果您还记得，构建加法器的一种方法是使用表达式分配两位。这种用法更常见。

# 试验台使模拟成为可能

在将设计提交给 FPGA 之前，您可能需要对其进行仿真。在模拟过程中调试要容易得多，因为您可以检查一切。当 Verilog 模拟器运行时，它遵循考虑到所有东西如何同时运行的时序规则，因此行为应该完全是您的 FPGA 将做的。

许多模拟器唯一不会做的事情是考虑芯片本身的时序(尽管使用正确的工具，您也可以模拟)。例如，您的设计可能依赖于时钟沿之前的输入变化(例如触发器的建立时间)，但由于芯片上的路由，输入不会及时变化。

对于大芯片和高速度来说，这种时序冲突是一个真正的问题。对于这种小电路，这应该不是问题。现在，我们可以假设，如果模拟工作，FPGA 应该以同样的方式工作。

为了测试我们的代码，我们需要一个测试平台，它只是向我们的被测单元(在这种情况下，是整个设计)讲述一段像外界一样工作的 Verilog 代码的一种方式。代码永远不会合成，所以我们可以使用奇怪的 Verilog 特性，这些特性通常不会在我们的常规代码中使用。

首先要做的是为测试平台创建一个模块(名称并不重要),并创建我们想要测试的模块的一个实例:

```
`default_nettype none
```

```
module tb;
 reg  a, b;
 wire led1, led2, led3, led4, led5;
 demo dut(led1,led2,led3,led4,led5,a,b);
```

请注意，对于我们想要提供给被测设备的每个输入都有一个`reg`，对于它将要驱动的每个输出都有一个`wire`。这意味着所有这些`reg`变量都需要根据我们的测试条件进行设置。

这些变量需要初始化。Verilog 提供了一个初始块，通常对综合无效，但将成为大多数测试平台的主要部分。这是它的第一部分:

```
 initial
 begin
   $dumpfile("dump.vcd");
   $dumpvars(0, dut);
```

```
   a=1'b0;
   b=1'b0;

```

这两个$语句告诉 testbench 将变量从被测设备转储到一个名为 dump.vcd 的文件中(这也是 EDAPlayground 查找它的地方，所以除非您使用自己的 Verilog 模拟器，否则不要更改它)。我们可以检查任何被丢弃的东西。您还可以使用$display 打印东西，但是我在这个测试中没有这样做。

接下来你需要的是一些测试案例刺激。在计数器的情况下，除了时钟，你不需要任何东西。但是加法器相关电路需要一些值:

```
#2
 a=1'b1;
 #4
 b=1'b1;
 #4
 a=1'b0;
 #4
 b=1'b0;
 #4
 $finish;
 end
```

所以一开始，a=1，b=0。然后经过 4 个周期，a=1，b=1。再过 4 个周期后，a=0，b=1。那么 a=0，b=0。$finish 语句导致模拟结束。如果没有这一点，时钟发生器将导致模拟永远继续下去。

您可以在 [EDAPlayground](http://www.edaplayground.com/x/DXe) 上找到代码和测试平台(您甚至可以从那里运行模拟)。运行模拟时，将出现一个波形(见下文)。如果你想知道更多关于它是如何工作的，看看下面的视频，我会一步一步地讲解。

[![logicdump](img/05a936218d645b6d1294dd4451d9a7e7.png)](https://hackaday.com/wp-content/uploads/2015/08/logicdump.png)

# 下次

在本系列的[明天部分，我将向您展示如何向设计和测试平台添加时序(时钟)逻辑。你很快就会看到，使用时钟是进行实用数字设计的重要组成部分。我还会有更多的 Verilog 要点。](http://hackaday.com/2015/08/20/learning-verilog-for-fpgas-flip-flops/)

[https://www.youtube.com/embed/Oq8Z0eK0Fmg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Oq8Z0eK0Fmg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

# 精选教程

如果您正在寻找详细的 Verilog 教程，请尝试以下内容:

*   [Doulos(EDA playground 的主持人)有一套非常专业的教程](https://www.doulos.com/knowhow/verilog_designers_guide/)
*   [另一个教程设置为自学课程](http://vol.verilog.com/)
*   EDAPlayground 的创建者在 YouTube 上有一个系列会很有帮助，尤其是如果你正在使用 EDAPlayground 的话

[你也可以阅读本系列的下一篇文章](http://hackaday.com/2015/08/20/learning-verilog-for-fpgas-flip-flops/)。

[https://www.youtube.com/embed/eXb8prknDKg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/eXb8prknDKg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)