# 绑着这么多硬件，机器人几乎不能移动

> 原文：<https://hackaday.com/2012/12/24/robot-can-barely-move-with-so-much-hardware-strapped-to-it/>

![web-server-robot](img/51a952ab092cfbf8b53e2bae9b9e5090.png)

我们认为(安德烈·什克拉巴)需要开始寻找一个更强大的汽车平台。这个小机器人身上绑了如此多的硬件，以至于马达几乎跟不上。但是只需一点点帮助，它就可以在房子里四处走动，而且需要大量的连接和计算能力。

上面的白棍是单板电脑。MK802 Mini 配备了 A10 处理器和高达 1g 的内存。就在它的下面是一个 USB 集线器，它位于 USB 电池组的顶部。这为计算机供电，并使他能够插入多个 USB 设备。机器人底盘来自 Pololu。它使用 Arduino 和电机护罩来移动，通过 USB 向它发送命令。

这种设置使得编程非常容易。这里[Andrej]有一个键盘和 HDMI 显示器插入做一点工作。当不编码时，它可以断开连接并通过网络驱动。他使用 MK802 和 node.js 上的 Apache 服务器实现了这一点。

[https://www.youtube.com/embed/19X0anqR_rM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/19X0anqR_rM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)