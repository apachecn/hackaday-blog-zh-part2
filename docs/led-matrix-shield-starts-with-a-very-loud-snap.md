# LED 矩阵屏蔽启动时会发出很大的咔哒声

> 原文：<https://hackaday.com/2012/05/02/led-matrix-shield-starts-with-a-very-loud-snap/>

![](img/238cf61587314102b75a4cd3b187bc55.png "9x9-led-matrix-with-clapper")

我们看到很多 LED 矩阵项目。它们很有趣，在构建过程中你可以学到很多基础知识。但是这一个与众不同。为他的 Arduino 建造了一个奇怪大小的声控矩阵盾。就在那里，盾牌是一大块原型板，但是你可以看到 Arduino 从它的顶部露出来。

现在我们说大小奇怪，因为 9×9 矩阵对于 8 位微控制器来说没有多大意义。没有原理图，但在休息后的剪辑中，他提到列和行由十进制计数器和移位寄存器驱动，这使得轻松驱动 9 位成为可能。电路板上还应注意矩阵右侧上方的垫圈。这是一个触摸感应复位按钮。但主要的控制机制是一个克拉珀克隆电路。只需打响指，它就可以打开或关闭项目。[Rtty21]基于[这种逐步声音输入构建](http://www.instructables.com/id/How-to-make-a-CLAP-ON-CLAP-OFF-circuit-from-scra/)的设计。

[https://www.youtube.com/embed/lb3sMFERdmk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lb3sMFERdmk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)