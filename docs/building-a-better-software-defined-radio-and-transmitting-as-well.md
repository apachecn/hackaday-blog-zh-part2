# 构建更好的软件定义无线电(以及传输)

> 原文：<https://hackaday.com/2012/10/24/building-a-better-software-defined-radio-and-transmitting-as-well/>

![](img/33f872c851b50f0c94471d2f89c33e5f.png "HackRF")

到目前为止，大多数黑客读者应该已经熟悉今年软件无线电的最新进展。通过一个简单的 USB 电视调谐器加密狗，它可以接收调频广播，卫星的 GPS 数据，甚至头顶上飞行的飞机的遥测数据。不过，这种设置有一个限制:只能接收。杰出的黑客迈克尔·奥斯曼(Michael Ossmann)正在寻找一种更好的软件定义无线电，称为 [HackRF](http://ossmann.blogspot.com/2012/06/introducing-hackrf.html) 。

HackRF 是一个令人难以置信的雄心勃勃的项目——能够接收 100 MHz 到 6 GHz 之间的任何信号(这包括从 FM 无线电波段的顶端到无绳电话、手机、WiFi，以及基本上在过去 15 年中商业化的任何无线电技术), HackRF 还能够进行 T2 发射。是的，有了 HackRF，您可以构建自己的软件定义的 WiFi 模块，或者只是广播虚假的 GPS 信息。

与我们玩过的 20 美元的电视调谐器 SDR 加密狗相比，HackRF 并不便宜。[莫斯曼]估计他能以大约 300 美元的价格卖掉这个设备。这是一个相当大的变化，但比专业的、商业的 SDR 解决方案要小得多。

SDR 状态的一个非常酷的进步，但是理性要求我们必须建议每个想要 HackRF 的人现在就开始学习他们的业余无线电考试。成为一名有执照的无线电操作员不会阻止你任何形式的恶意企图，但至少有了执照就有可能知道你在做什么坏事。

你可以在维基上查看 gits 上的 HackRF [以及](https://github.com/mossmann/hackrf/wiki)[当前的硬件设计](https://github.com/mossmann/hackrf)