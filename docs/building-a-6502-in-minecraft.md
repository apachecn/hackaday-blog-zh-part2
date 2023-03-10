# 在《我的世界》建一栋 6502

> 原文：<https://hackaday.com/2012/05/20/building-a-6502-in-minecraft/>

我们承认，我们没有像过去那样关注《我的世界》；自从我们在《我的世界》看到令人惊讶的东西已经有一段时间了，但是[eloraam]的 [6502 模拟器](http://gamegenus.blogspot.com/2012/04/6502-emulator-in-minecraft-runs-forth.html)(她的[红色力量《我的世界》模块](http://www.eloraam.com/?p=263)的一部分)拿走了蛋糕。

RedPower mod 为《我的世界》增加了许多工业技术。水泵、太阳能电池板和移动积木的气动管道是这个模型的主要组成部分，但随着一台完全仿真的 6502 电脑的加入，《我的世界》从一种不合时宜的中世纪主题蒸汽朋克美学转变为一种全面的机器时代，到处都是大型机的风格。

红色能量模块 6502 部分的核心是三个可加工的模块；CPU、显示器和磁盘驱动器。所有这些区块通过带状电缆连接在一起，可以与《我的世界》宇宙中的其他区块相互作用。CPU 是一个仿真的 6502，借用了 65816 的一些指令，并增加了 MUL 和 DIV。用汇编语言给这台计算机编程是可能的，但是操作系统中的第四个解释器使编程变得更容易一些。

自从我们第一次看到《我的世界》制造的 CPU 的雏形已经过去了将近两年，但是这款 mod 将一切提升到了一个新的水平。实际上，这和[【notch】目前正在开发的游戏](http://hackaday.com/2012/04/08/getting-12-year-olds-to-learn-assembly-programming/)没有太大的不同；两者都有一个模仿 80 年代的电脑，可以做你所有的游戏内投标。我们无法想象还有什么比这更好的方式让我们再次迷上《我的世界》，我们不得不称赞[eloraam]所做的一些非常棒的工作。

休息之后是一个 23 分钟的关于 RedPower CPU 功能的教程，由《我的世界》爱好者演示。

[https://www.youtube.com/embed/vb0Q9htsbBI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vb0Q9htsbBI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)