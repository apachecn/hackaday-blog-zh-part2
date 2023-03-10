# Linux 画框充当无线树莓 Pi 显示器

> 原文：<https://hackaday.com/2012/06/28/linux-picture-frame-serves-as-wireless-raspberry-pi-display/>

![](img/f18559dfc49487c6e153d1b40ae3a5e6.png "wireless-display-for-rpi")

这里有一个新颖的方法来添加一个显示到您的树莓 Pi。[Chris Bryden]决定[使用蓝牙来提供无线显示](http://www.cjb.im/2012/06/raspberry-pi-wireless-display-using.html)，而不是使用有线显示——通过 HDMI(可以通过简单的硬件适配器连接 DVI 端口)或复合视频输出。这真的取决于你可用的硬件。他在[为一首歌抢购了一个可折叠的数码相框](http://hackaday.com/2012/01/10/this-digital-picture-frame-runs-linux-better-than-you-might-think/)，并在这个项目中使用了 320×240 的显示器。

在上图中，你可以看到插入 RPi 的 USB 接口。这是一个蓝牙适配器，数码相框上有一个与之匹配的。两者以这种方式联网后,[Chris]开始设置 VNC，让他可以通过网络调出 X 桌面。

这是我们见过的蓝牙协议的最佳用途之一，小屏幕比使用简单的字符显示提供了巨大的优势。