# 用手表来控制 Pacman 女士

> 原文：<https://hackaday.com/2012/07/20/using-a-watch-to-control-ms-pacman/>

![](img/6e9d42663db0385c4e6cb3616a2caf3a.png "pac")

最近，[Alan]拿出了' ol Atari 2600，带着一点儿 *Yar 的复仇*和*的冒险*重温他的童年，但在看了他的新 TI EZ430 Chronos 手表后，他认为他可以从这个经典的游戏系统中添加一点运动控制。他用这款手表中的加速度计通过倾斜手腕来[玩*吃豆人*游戏，这是一个令人敬畏的构造，真正展示了他的新腕戴设备的威力。](http://www.youtube.com/watch?v=TcZBFHLC4U4)

这款手表运行的是普通固件，通过连接到电脑 USB 端口的射频模块与电脑通信。加速度计数据被输入 VB.net 应用程序，将手腕的运动转换为向上、向下、向左和向右的命令。这些命令然后通过串行端口发送到 Arduino，将这些命令翻译成 Atari 操纵杆端口可以理解的内容。

当然，这可能是玩吃豆人女士的一种迂回方式，但考虑到 TI Chronos 已经被用于非常严肃的工作，如[阻止 SIDS](http://hackaday.com/2012/07/04/ti-chronos-watch-monitor-your-sleeping-infant/) 和[帮助足球裁判](http://hackaday.com/2012/07/04/fifa-looks-at-electronic-augmentation/)，我们很高兴看到这款简洁的手表有更轻浮的应用。

您可以在休息后查看[Alan]的视频，或者在这里获取 VB 和 Arduino 源[，在这里](https://www.box.com/s/8c0d8e6cd782ecf1599a)获取[。](https://www.box.com/s/9c46d065da86a6800521)

[https://www.youtube.com/embed/TcZBFHLC4U4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TcZBFHLC4U4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)