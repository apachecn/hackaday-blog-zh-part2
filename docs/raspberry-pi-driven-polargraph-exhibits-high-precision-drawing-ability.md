# Raspberry Pi 驱动的 Polargraph 显示出高精度绘图能力

> 原文：<https://hackaday.com/2012/11/16/raspberry-pi-driven-polargraph-exhibits-high-precision-drawing-ability/>

![](img/935af2aca78c0b1b273c23808be784ef.png "rpi-polargraph")

这张[极坐标图在写字板上画出了一些神奇的形状](https://code.google.com/p/gocupi/)。这部分是由于两个步进电机和触控笔使用的安装支架。但是，为了计划下一组动作，将速度考虑在内的代码也是值得称赞的。

[Go 语言](http://golang.org/)用于将数据翻译成两个电机的步进命令。该命令流通过 RPi 板和 Arduino 之间的串行连接传送。Arduino 只是将这些步骤推给电机控制器。RPi 的加入提供了进行这种平滑设计所需的马力。这在[布兰登·格林的]帖子的后半部分有所解释。该技术在大多数情况下使用恒定的加速度、速度和减速度，防止悬挂的触针发生任何类型的振动。但是，当没有足够的空间来平稳地加速或减速时，也有应急措施。

你可以捕捉到一个很短的硬件剪辑，在休息后嵌入的视频中绘制了一个紧密的螺旋。

[https://www.youtube.com/embed/4eZVGvScbqg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4eZVGvScbqg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)