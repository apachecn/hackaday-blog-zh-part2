# 二维码向你敞开大门

> 原文：<https://hackaday.com/2012/09/17/qr-code-opens-doors-to-you/>

![](img/ccc5f40c1d3af607891c2adc97771f04.png "QR-code-opens-door-to-you")

【Jeremy Blum】来信分享[他的 LibeTech 二维码门锁项目](http://www.jeremyblum.com/portfolio/libetech/)。他在康奈尔大学高年级时和他的三个同学一起开发了它。它试图摆脱磁卡锁，转而支持基于 QR 码进行身份验证的光学锁。

他在这里使用的硬件肯定成本过高，但我们确信这个概念可以大大简化。在这种情况下，运行嵌入式 Linux 的 BeagleBone 监控来自网络摄像头的提要。当它检测到一个二维码时，它会将它与一个数据库中的许可钥匙进行比较，然后为你打开门。

这种技术有一些问题，一个是攻击者可能在你不知道的情况下获得你的钥匙的有用照片。但是现在使用的大多数酒店锁甚至没有 T1 的安全。从好的方面来说，你房间的钥匙可以通过电子邮件发送给你，你可以在任何带屏幕的设备上使用，或者打印在一张纸上。

休息之后，您可以看到[Jeremy 的]演示视频。

[https://www.youtube.com/embed/C8ZT-4VX1BE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/C8ZT-4VX1BE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)