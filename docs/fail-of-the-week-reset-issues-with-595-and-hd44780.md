# 本周故障:重置 595 和 HD44780 的问题

> 原文：<https://hackaday.com/2014/02/27/fail-of-the-week-reset-issues-with-595-and-hd44780/>

![fotw-reset-issues-595-character-lcd](img/856751b3f360c2f70b639d18a253140f.png)

我们真的很想看到硬件黑客走出现有 Arduino 库的安全和完美的边界。一个例子是[Matteo]认为有效的项目:[使用移位寄存器驱动字符 LCD](http://hackaday.com/2014/02/03/controlling-alphanumeric-lcds-with-three-wires/) 。这可能是一种理想的方式，因为它将 GPIO 的使用从六个减少到三个。如果你不记得本月早些时候看过那张照片，那就再看一眼。要点是[Matteo]黑进了 LiquidCrystal 库中的一个函数来实现它。

这是一个真正的大失败，因为问题没有立即显现出来，并且很难可靠地重现。[LCD 不稳定取决于 Arduino 板如何复位](http://www.alpheratz1991.com/2014/02/3-wires-lcd-display-part-2-help-me-to.html)。将 Arduino 连接到电脑时，屏幕不会工作，直到您按下重置按钮。但是重复按复位按钮，你会得到一个不起作用的屏幕，还有上面看到的胡言乱语。

这里没什么可说的，但我们认为陈述你对故障的理论并提出测试/修复问题的建议会很有趣。这可能是很多事情，显示器上的控制器搞混了，595 丢失了一个边缘(或类似的事情)。您是通过硬件(即:避免电压骤降的电容器)、软件问题(启动后需要更长的延迟)还是两者的结合来解决这个问题？

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**