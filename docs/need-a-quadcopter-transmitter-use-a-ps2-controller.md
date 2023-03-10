# 需要四轴飞行器发射器？使用 PS2 控制器！

> 原文：<https://hackaday.com/2012/07/16/need-a-quadcopter-transmitter-use-a-ps2-controller/>

![](img/e9ee550db9e9f80f291d367208e7e7b1.png "tx")

在[Pyrofer]造出四轴飞行器后，他购买了中国制造的廉价 6 通道发射机。不幸的是，那个发射器很糟糕，所以他拿了一个旧的 PS2 控制器[做了自己的](http://www.pyrofersprojects.com/blog/ps2pad-tx/)。

对于他的构建，[Pyrofer]拿出模拟棒，并将其连接到控制器手柄中的 AVR。AVR 向一个由小型 LiPo 电池供电的 2.4 GHz 无线电发射机发送命令。在控制器的肩膀按钮后面增加了几个轻触开关，[Pyrofer]有四个控制轴，还有几个按钮可以改变他的四轴飞行器的模式。

这种构建确实无法与我们见过的一些令人敬畏的 [DIY RC 发射器](http://hackaday.com/2012/07/11/remote-control-with-an-xbee-and-a-propeller/)相提并论，但我们不得不称赞[Pyrofer]提出了一种非常简单和容易的构建。几乎每个人都有一个 PS2 或 XBox 控制器，加上一些额外的硬件，很容易就能得到一个像样的遥控器。

[Pyrofer]使用了一个名为 [Funkenschlag](https://github.com/wertarbyte/funkenschlag/) 的项目来产生 PPM 信号，所以如果你觉得有必要复制这个项目[，当你完成后在](http://hackaday.com/contact-hack-a-day/)中发送它。