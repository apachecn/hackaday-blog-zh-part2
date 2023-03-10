# 轻松控制 Arduino Mega 的 LCD

> 原文：<https://hackaday.com/2013/07/24/easy-lcd-control-for-arduino-mega/>

![arduino-mega-easy-lcd-adapter](img/a90d15c03cdc0725cfc7f2df5f68c92b.png)

[安迪·布朗]来信展示了他一直致力于将廉价显示器连接到 Arduino Mega 的 TFT LCD 适配器。

这些薄膜晶体管液晶显示屏可以在易贝花几美元买到。但它们更适合工作在 3.3V 电平的 16 位微控制器。他的适配器板直接插入 Mega 的双排引脚接头，使得用 5V 运行的 8 位芯片控制这些更容易。

有几个因素导致了这种情况。首先，他加入了电平转换器芯片来处理 3.3V/5V 问题。其次，他使用 latch 芯片将 Arduino Mega 上的 8 个引脚转换为显示器上的 16 个引脚。这些芯片有一个锁存引脚，当输入引脚改变时，它将输出值保存在存储器中。他设法使用 LCD 协议要求的片选(CS)线来驱动其中一个芯片上的锁存器。这意味着你不会失去任何额外的引脚。

使用 Arduino 显示器的另一种方式是使用 TFT 屏幕的智能控制器。

[https://www.youtube.com/embed/TlVMz90AYHs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TlVMz90AYHs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)