# 使用 I2C 地址作为芯片选择

> 原文：<https://hackaday.com/2015/03/27/using-i2c-addresses-as-chip-selects/>

I2C 有一个 7 位的地址空间，你会想“我什么时候需要在一对线上有超过 127 个设备？”因此，订购某些器件时，发现它们对于任何给定的器件类型都有一个、两个或三个用户可配置的地址引脚。在你的项目中，你需要不止四个或八个电容式传感器按钮。你是做什么的？

如果你是 reader [Marv G]，你会[跳出框框](http://emgoz.blogspot.de/2015/03/i2c-plus-chip-select.html)思考，并意识到你可以通过微控制器切换地址引脚的高低来动态改变地址。也就是说，每个器件可以使用一个 I2C 地址引脚作为片选信号，就像 SPI 一样。

就这样，真的。[Marv G]在他的文章中介绍了所有其他可能的选择，它们都是令人讨厌的:多条 I2C 总线，一个多路复用器，购买不同的传感器，或者更换微型计算机。没有一种方法像多走几条线并用你的微处理器来回切换那样简单。

我们甚至建议，您可以使用移位寄存器或 1/N 解码器芯片来扇出这些芯片选择线，具体取决于您需要对多少 I2C 器件进行芯片选择。(我们考虑的是 74HC595 或者 74HC154。)

在这个过程中，我们发现了由[LadyAda]提供的一系列常见外设的地址引脚数量的漂亮[列表，以防你不相信我们这个问题有多普遍。该列表中有多少设备有一个(1！！)地址 pin？](http://www.ladyada.net/library/i2caddr.html)

在文章的最后，[Marv G]询问是否有其他人以前想到过这个芯片选择技巧。我们没有。这是你在评论中耍小聪明的机会。