# 永久乒乓

> 原文：<https://hackaday.com/2013/04/10/perpetual-pong/>

![perpetual-pong](img/3367dbc2465927e79816d0d2823a451e.png)

[杰夫·乔雷]写信来炫耀他制作的这个永久乒乓装置。6×10 的 LED 矩阵充当 Pong 的游戏板，但没有控件。董事会简直是在和自己作对。这就像是[一个没有时钟的乒乓时钟](http://hackaday.com/2011/02/09/pong-clocks-using-led-matrix-modules/)。

该设备的大脑是 PIC 16F684，它直接驱动显示器的六行。他用一个十进制计数器(CD74HC401)一次扫描一行。现在，你希望在这块原板的下面找到什么？点对点线路的老鼠窝？如果是这样，你会失望的。[Jeff]花时间在 Eagle 中生成原理图和电路板布局。在此期间，他知道他将使用 protoboard，因此艺术品被设计为尽可能使用焊料桥接。他最终得到的是你能找到的最干净的多重一次性项目之一。看它在跳跃之后的动作。

[https://www.youtube.com/embed/6d0Rum2Th7A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6d0Rum2Th7A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)