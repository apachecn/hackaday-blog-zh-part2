# DUO Decimal——简约的单板计算机

> 原文：<https://hackaday.com/2014/06/23/duo-decimal-a-minimalist-single-board-computer/>

![duodecimal](img/fa100edd8f368f9d762b6ca5ce90c81d.png)

如果你曾经努力把你的程序装进一个微型计算机的 ram 和 ROM 中，你会欣赏[杰克]的创造，二进制的。DUO Decimal 是运行在 Atmel ATtiny84 上的小型单板计算机。84 具有 8KB 闪存、512 字节 SRAM 和 512 字节 EEPROM。不像过去那么糟糕，但以今天的标准来看还是很紧。

用户通过两个按钮向 DUO Decimal 输入。输出通过一个 7 段数字 LED 显示器。对于输入长程序来说不是最容易的，但与过去的开关和闪光灯不相上下。3 位 GPIO 可用于连接您自己的电路。

[Jack]不仅仅是设计了一块板，他还设计了整个语言。DUO Decimal 是用一种称为 DUO Decimal 数字代码(DDNC)的解释语言编程的。有 47 个 DDNC 命令，涵盖了从基本数学到列表操作的所有内容。程序可以通过按键进入，也可以通过 AVR isp 接口下载，节省你的指尖。包括 DDNC 解释器在内的完整的二进制 C 代码可以在[杰克的]网站上找到。

[Jack]创建了几个示例 DDNC 程序，包括一个带三角学的 6 函数计算器、一个 Mandelbrot 集合测试器和一个石头剪刀布游戏的实现。甚至还有一个平台动作游戏，尽管单个 7 段显示器上的图形至少可以说是简单的。

[https://www.youtube.com/embed/G5EbSjDjMG4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/G5EbSjDjMG4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)