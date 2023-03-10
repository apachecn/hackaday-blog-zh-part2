# 声学延迟线存储器

> 原文：<https://hackaday.com/2014/01/07/acoustic-delay-line-memory/>

回到过去，计算机既是模拟的又是数字的，制造 RAM 实际上非常困难。没有晶体管，建立记忆系统的唯一纯电子手段是真空管；这本来是可以做到的，但对于任何可观的内存量来说，都意味着数量惊人的显像管、功率和高故障率。

早期 RAM 的解决方案之一是一种叫做延迟线的东西。该设备使用超声波传感器通过介质(通常是加热到 40℃的充汞管)发送脉冲，并在另一端读出脉冲。发送和接收脉冲之间的时间刚好够用作一个非常大的小容量 RAM。

对于一个简单的电子项目来说，装满数百磅水银的加热管不是你想要的东西。然而，你可以用一个无线电室电子学习实验室、一个扬声器和一个麦克风来建造一个。

[Joe]使用运算放大器设计了他的延迟线，以放大在空气中传播的声脉冲序列。压缩器拾取这些脉冲，并将其发送到触发器。十进制计数器和振荡器提供脉冲的定时，并提供将每一位放入延迟线的方法。当按下电子实验室上的一个按钮时，一个“滴答”信号被发送到扬声器，穿过[Joe]的地下室，进入麦克风，然后回到电路。

整个装置能够在空气中存储 10 位信息，数据可以方便地在示波器上显示出来。这不是一种以任何方式、形状或形式存储数据的实用方法，但它是对数字化一切之前的世界的有趣窥视。

下面视频。

[https://www.youtube.com/embed/a5hOmPdxw0U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/a5hOmPdxw0U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)