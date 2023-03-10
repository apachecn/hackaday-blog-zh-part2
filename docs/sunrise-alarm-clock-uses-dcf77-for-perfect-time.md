# 日出闹钟使用 DCF77 获得完美的时间

> 原文：<https://hackaday.com/2012/12/06/sunrise-alarm-clock-uses-dcf77-for-perfect-time/>

![sunrise-alarm-clock-dcf77](img/7a46d038294973c044e2c3022e3d056c.png)

这是一款走时准确的日出闹钟。它是由 Renaud Schleck 设计和建造的，他还发表了一篇文章详细介绍了这个过程。

正如你所看到的，透明外壳内的一系列白色发光二极管提供了模拟的日出。随着白天变短，夜晚变长，我们确实看到了让你的闹钟在把你从睡眠中惊醒之前照亮房间的好处。说起来，那个警报声似乎是他设计中的薄弱环节。他用一个经过电容平滑的方波来驱动机箱两端的扬声器。我们没有听到一个例子，但我们想象这不是最温柔的声音。

设计的其余部分做得相当好。他使用的是 4×20 字符的 LCD 显示器，并使用 PWM 调节背光。DCF77 无线电从原子钟信号向运行时钟的 MSP430 芯片提供数据。甚至还有备用电池以防停电。

我们昨天刚刚看到一个项目，旨在通过 DCF77 无线电提高信号质量。

[via [Reddit](http://www.reddit.com/r/electronics/comments/13znuz/dcf77_controlled_sunrise_alarm_clock_i_built/)