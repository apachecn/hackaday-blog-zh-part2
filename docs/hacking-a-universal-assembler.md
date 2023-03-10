# 破解通用汇编程序

> 原文：<https://hackaday.com/2015/08/06/hacking-a-universal-assembler/>

我总是嘲笑那些在工具箱里放着多功能工具的人——那些现代的瑞士军刀。对我来说，多功能工具的全部前提是它们让我不用去使用工具箱。如果我有时间去修车厂，我会找到合适的工具。

不是说我不喜欢好的多功能工具。他们是完成工作的权宜之计。这就是我对 [axasm 的感觉——我一直在一起破解的一个通用汇编器](https://github.com/wd5gnr/axasm)。称之为交叉汇编器黑客并不公平。这是一个巨大而丑陋的攻击，但它确实完成了任务。如果我需要一些严肃的东西，我会去工具箱拿一个真正的汇编程序，但有时你只想用你口袋里的东西。

## 为什么是交叉汇编程序？

[![A cross compiler is a compiler capable of creating executable code for a platform other than the one on which the compiler is running. For example, a compiler that runs on a Windows 7 PC but generates code that runs on Android smartphone is a cross compiler.](img/f68f044a4ea9f70f25b9b31e65bb8e26.png)](https://en.wikipedia.org/wiki/Cross_compiler) 你可能想知道我为什么要写一个汇编程序。问题是，我喜欢设计定制的 CPU(通常在 FPGA 上用 Verilog 实现)。这些 CPU 有独特的指令集，这意味着没有现成的汇编程序。您可以定制一些表驱动的汇编器，但是您必须学习该工具的一些晦涩难懂的专用语法。我的目标不是写一个汇编程序。那是为了给我的新 CPU 写一些代码。

对于我的第一对 CPU，我只是用 C 或 awk 写了一个汇编器。我注意到他们看起来都有点相似。我使用过的几乎每一种汇编语言都有一个非常规则的格式:一个可选的标签后跟一个冒号、一个操作码助记符，可能还有几个逗号分隔的参数。分号标记注释。你还会得到一些非常常见的特殊命令，比如 ORG、END 和 DATA。这让我开始思考，这通常是很危险的。

## 特雷·哈克

C 预处理器名声不好，可能是因为它像炸药一样。它非常有用，但也非常危险，尤其是在坏人手里。我想到，如果我的汇编语言看起来像 C 宏，我可以很容易地从一个固定的框架创建一个定制的汇编程序。可能所有我的目标处理器都有相对较小的内存(以 PC 标准来看),所以为什么不在 C 程序中使用宏来填充数组呢？然后，编译器将完成所有工作，一些标准例程可以将结果以二进制或英特尔十六进制格式或您可以想象的任何其他格式输出。

我的计划很简单:使用 awk 脚本将传统的汇编格式代码转换成宏。这将转换一行，如下所示:

```
      add r1,r2
```

变成这样的宏:

```
     ADD(r1,r2);
```

注意操作码总是被强制大写。标签需要一些特殊的处理。当汇编脚本找到一个标签时，它将一个 DEFLABEL 宏输出到一个特殊的额外文件中。然后，它将一个标签宏写到主文件中。这是必要的，因为你可能在定义标签之前就使用了它(向前跳转),汇编程序需要提前知道它们。

## 结果呢

与普通的汇编程序不同，脚本的输出文件不是机器码。汇编程序的标准源代码中包含了两组 C 语言宏。驱动程序脚本协调了整个过程。它运行脚本，调用编译器，然后执行生成的(临时)程序(向它传递您指定的任何选项)。标准源代码只是得到一个填充了机器代码的缓冲区，并以几种可用格式之一发出它。你可以在下面看到整个流程。

[![axasm](img/61e08d9ed05b03a0c460b7f7d036b63f.png)](https://hackaday.com/wp-content/uploads/2015/08/axasm.png)

如果这还不够清楚的话，生成的程序有一个功能:使用某种格式用机器码打印出你的特定汇编语言程序。就是这样。您不保存可执行文件。一旦他们跑了，他们就不再有用了。

汇编程序用来生成代码的函数是`genasm()`。驱动程序调用它两次:一次是为了计算所有标签值，第二次是为了实际发出机器代码。genasm 函数是在汇编代码之外创建的。每个处理器定义都有一个 ORG 宏来设置一切，包括 genasm 函数头。END 宏将它和其他一些内务处理一起关闭。

## 配置

那么，关键是配置宏文件。由于脚本将所有内容都转换为大写，所以宏文件必须使用大写的操作码(但程序不一定要这样)。正如我提到的，你必须以某种方式生成 genasm 函数，所以这通常需要一个 ORG 和一个 END 宏。这些通常会建立一个假的地址空间(我的处理器都没有超过 4MB 的程序存储，所以我可以很容易地在 PC 上创建一个数组)。然后，我将为每种指令格式定义一个宏，并使用它来定义更多用户友好的宏。ORG 宏还必须在 _solo_info 结构中设置一些配置项(比如字长和机器码数组的位置)。

因为 ORG 设置东西一次，不能重复使用。这意味着我通常提供一个只移动到新地址的 REORG 宏。有时候黑客需要一点妥协，这就是其中之一。

作为一个例子，考虑[心脏](https://en.wikipedia.org/wiki/CARDboard_Illustrative_Aid_to_Computation)。这是一台由纸板制成的简单计算机，贝尔实验室曾在 20 世纪 60 年代向学校提供计算机教学(你仍然可以买到一些，我也在 [FPGA](http://opencores.org/project,vtach) 中重新制作了它)。以下是心脏的部分组织定义:

```
#define ORG(n) unsigned int genasm(int _solo_pass) { \
 unsigned _solo_add=n;\
 _solo_info.psize=16; \
 _solo_info.begin=n; \
 _solo_info.end=n; \
 _solo_info.memsize=MAXMEM; \
 _solo_info.ary=malloc(_solo_info.memsize*_solo_info.psize); \
 _solo_info.err=(_solo_info.ary==NULL)
```

地址是 ORG 语句的参数)，程序大小是 16 位。现在数组的开始和结束也是 n，但这当然会改变。

__setary 函数在数组中加载机器代码值，其他指令使用该宏使它们易于编写:

```
#define INP(r) __setary(_solo_add++,bcd(r))
#define LOD(r) __setary(_solo_add++,bcd(100+(r)))
```

因为 CARDIAC 是 bcd 机器，所以 BCD 宏有助于以正确的格式创建输出数字(例如，十进制的 100 变成十六进制的 100)。这并不常见，但它确实证明了通过在定义文件中编写一点 C 代码，您可以适应几乎任何事情。

## 运转

一旦有了汇编语言程序和合适的处理器定义，从命令行运行 axasm 就很容易了。如果您只是运行 axasm，您将得到以下使用消息:

```
Usage: axasm [-p processor] [ -H | -i | -b | -8 | -v | -x ] [-D define] [-o file] inputfile
 -p processor = processor.inc file to use (default=soloasm)
 -D = Set C-style preprocessor define (multiple allowed)
 -H = Raw hex output
 -i = Intel hex output
 -v = Verilog output
 -x = Xilinx COE format
 -b = Binary raw (32-bit only)
 -8 = Binary raw (8-bit only)
 -o = Set output file (stdout default)
```

p 标志指定了您想要使用的定义。该程序可以输出原始十六进制、Intel 十六进制、Verilog、Xilinx COE 格式和原始二进制(如果您想将其转换为 8080 的八进制，请使用 od)。

## 有什么意义？

以这种方式扭曲 C 预处理器似乎有点奇怪，但它确实有很多优点。首先，你可以用一种舒适的语言定义你的 CPU 指令集，并在函数和宏中使用强大的构造来完成工作。第二，你可以使用 C 编译器的所有特性。例如，常量数学表达式工作正常。

您甚至可以使用 C 代码来生成您的汇编程序，方法是在 C 代码行前面加上#(预处理器行有两个#字符)。例如:

```
##define CT 10
# { int i; for (i=3;i<10;i++) LDRIQ(i); }
```

这将生成 LDRIQ 指令，I 从 3 到 9 不等。请注意，for 循环不会出现在您的代码中。它正在生成您的代码。您甚至可以使用预处理器在程序中定义简单的操作码或别名:

```
##define MOVE MOV
##define CLEAR(r) XOR(r,r)
```

当然，由于 AXASM 适用于定制处理器，所以您也可以定义标准处理器。Github 有 RCA1802、8080 和 PIC16F84 的定义。如果你创建了一个新的定义，请在 Github 上做一个 pull 请求并分享。

我不确定我是否想把这种技巧作为进行文本处理的通用技术。像炸药一样，它强大、有用，同时也很危险。然而，就像多功能工具一样，它非常方便，可以完成工作。如果你需要复习 C(和 C++)预处理器，看看下面的视频。

[https://www.youtube.com/embed/ZYpvz9ZAwDI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZYpvz9ZAwDI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)