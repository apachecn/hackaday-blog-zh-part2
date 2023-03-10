# 在线 SD 卡开关

> 原文：<https://hackaday.com/2014/06/08/the-in-circuit-sd-card-switch/>

![SDISP](img/f09b6d607454a27395449c8744ac0469.png)

几乎每个问题都有可能设计出解决方案，即使你正在处理一个可能只适用于你自己的非常特殊的问题。[Joel]希望能够使用新的引导加载程序或文件系统对他的 BeagleBone 中的 microSD 卡进行编程，而无需从目标板上移除 SD 卡。这是一个特殊的要求，很可能没有一种产品甚至电路可以实现这样的功能。这意味着[Joel] [将需要滚动他自己的板](http://www.linuxinternals.org/blog/2014/06/04/a-microsd-card-remote-switcher/)来完成任务。

该板非常简单，包含一个 microSD 插座、两个用于[的扩展接头、一个用于计算机和嵌入式板的 microSD 嗅探器](https://www.sparkfun.com/products/9419)、一个 FTDI 接头和一对 [4 位多路复用器/多路分离器](http://www.ti.com/product/sn74cbt3257)。该设备的操作相当简单:沿 FTDI 电缆发送信号，电路板将板载 SD 卡从一个设备切换到另一个设备。

[Joel]有一段他的屏幕视频，显示他成功完成了在线 SD 卡读写。你可以看看下面。

[https://www.youtube.com/embed/StpIihVQ7oM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/StpIihVQ7oM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)