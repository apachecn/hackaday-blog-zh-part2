# Dan64:一种小型硬件 AVR 微机

> 原文：<https://hackaday.com/2015/04/07/the-dan64-a-minimal-hardware-avr-microcomputer/>

[Juan]给我们发来了他用 Arduino UNO (AVR ATmega328p)和一些板外 SRAM 制作的微型计算机的文章。这个非常简约。

看一下[示意图](http://www.usebox.net/jjm/dan64/dan64_v1-schematics.pdf) (PDF)。有一个 Arduino， [SPI SRAM](http://www.microchip.com/wwwproducts/Devices.aspx?product=23LCV512) ，一些用于电视视频输出的晶体管，以及一个用于键盘的 PS/2 连接器。就这样，真的。如果你手头有零件，它很容易在几分钟内在试验板上完成。将 Dan64 操作系统和虚拟机闪存到 AVR 中，您就可以开始了。

现在，我们最近在这里看到了一些基于 6502 的复古计算机，它们使用一个与微控制器配对的 T2 6502，但它们都是笨重的三芯片系统。[Juan]通过使用 AVR 中实现的 6502 虚拟机将整个射击比赛的零件数量减少到两个芯片，赢得了极简主义奖。

使用 6502 虚拟机在设计中是一个至关重要的选择，因为有 6502 交叉编译器可以让你在你的大型计算机上为微型计算机编译和调试代码，然后加载到微型计算机上运行。这使得开发微处理器不那么痛苦。

你问它如何加载程序？当然是老式的方法，使用音频文件。尽管他没有像过去那样使用堪萨斯城标准(T1 ),而是将数据编码成方波的长短脉冲。这可能不太可靠，但肯定节省了外部硬件。

[https://www.youtube.com/embed/gB_bxMhXWi4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gB_bxMhXWi4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

Dan64 的操作系统还能做什么？它有一个有限的外壳，包括一个 6502 汇编器和反汇编器，所以如果你愿意，你可以用本机汇编语言对微控制器进行动态编程。当然，没有通过 peek 和 poke 访问原始存储器的微控制器是不完整的。

看看[视频](https://www.youtube.com/playlist?list=PLvI1iQmfH6UMJUAfsyax0VGHfUk-wekLz)、[精心编写的说明书](http://www.usebox.net/jjm/dan64/dan64_v1-manual.pdf)、[代码](https://github.com/reidrac/dan64)。给自己造一台微型计算机，写一些软件，就像 1982 年一样。我们可以想出更糟糕的方式来浪费周末。