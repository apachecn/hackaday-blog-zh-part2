# 最基本的基本电脑

> 原文：<https://hackaday.com/2014/08/19/the-most-basic-basic-computer/>

如今，AVR 微控制器几乎可以做任何事情。闪烁的 led，处理传感器输入，发动机控制模块，现在，多亏了[Dan]，一个只有十个零件的[小型单片基本计算机](http://hackaday.io/project/2428)(其中四个是电容器)。

[丹]的自制电脑什么都有。ATmega 1284P 微控制器输出复合视频信号，并处理来自 PS/2 键盘的输入。微控制器以 16 MHz 运行，具有 7 kB 的程序存储器，可以使用单独的 EEPROM 存储数据。它还具有一系列 GPIO 引脚，用于与物理世界进行交互。

对于软件，微控制器运行一个名为 [Tiny BASIC](http://en.wikipedia.org/wiki/Tiny_BASIC) plus 的 BASIC 版本，这是一种精简的语言，可以放在 3 kB 的内存中。如果你是在 20 世纪 70 年代，或者如果你是在 21 世纪的 AVR 微控制器上编程，这是至关重要的。

我们已经看到了其他可以运行 BASIC 的 Arduinos 和 [AVR 型微控制器，但是这款有很好的外形和简洁的外观。这也是一个熟悉自制计算和 BASIC 编程语言的好方法！](http://hackaday.com/2011/08/28/basic-programming-on-an-arduino/)