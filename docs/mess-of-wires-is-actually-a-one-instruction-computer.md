# 乱七八糟的电线实际上是一台单指令计算机

> 原文：<https://hackaday.com/2012/09/05/mess-of-wires-is-actually-a-one-instruction-computer/>

如果你要建造自己的计算机，完全模仿你现在看到的计算机可能对你没有好处。驱动台式机或笔记本电脑的现代 x86 和 x64 芯片包含数百条单独的指令，ARM 驱动的设备中的 RISC CPUs 包含的指令几乎一样多。不，如果你打算建造你自己的计算机，你应该让它对你自己容易，就像[杰克·艾森曼]在建造 DUO Compact 时所做的那样，这是一台在试验板上制造的单指令集计算机。

顾名思义，单指令计算机只有一种操作位的方式，而不是几十或几百条单独的指令。对于 DUO Compact，[Jack]选择了 NOR 和 fork 条件指令。为 DUO Compact 编写的每一行汇编都有四条内存指令:源地址、目的地址、跳过地址 1 和跳过地址 2。[Jack]准确地解释了这个操作如何让他计算所有的东西:

> 执行指令时会发生三个步骤:
> 
> 1.  加载第一个和第二个地址的字节。也不是这些字节的总和。
> 2.  将步骤 1 的结果存储在第二个地址中。
> 3.  如果步骤 1 的结果是零，则跳到第四个地址的指令；否则，跳到第三个地址的指令。

似乎设计一台仅使用基本逻辑和内存芯片的单指令计算机还不够令人印象深刻，杰克甚至为他的系统、[编写了一个](http://www.ostracodfiles.com/compactpage/piston.html)[仿真器、](http://www.ostracodfiles.com/compactpage/emulator.html)编译器、[操作系统](http://www.ostracodfiles.com/compactpage/DUO%20OS%202.txt)，甚至还有一些程序，如平方根计算器和基于文本的冒险游戏。

无论如何，[Jack]已经完成了一个惊人的构建，但是我们被他提供的大量文档震惊了。他甚至还写了一篇教程，教你如何打造自己的双人组合。

休息之后，你可以看几段二重奏的视频。当然，如果你正在寻找一个需要解决的项目，我们非常欢迎你设计来自[DUO Compact 原理图](http://www.ostracodfiles.com/compactpage/compact%20schematic.png)的 PCB。我们当然会买一个。

[https://www.youtube.com/embed/IoMgCrOT3fU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IoMgCrOT3fU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/rqaZvJXc1Fk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rqaZvJXc1Fk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)