# USB 转串行适配器告诉你你在哪个 COM 端口

> 原文：<https://hackaday.com/2013/01/14/usb-to-serial-adapter-tells-you-what-com-port-youre-on/>

![xser](img/28d5469da20d9010488b460595ca0bc5.png)

由于我们大多数人早已过了硬件串行端口的时代，USB 转串行适配器已经成为黑客工具带上的支柱。虽然便宜又方便，但 USB 转串行适配器并不总是最容易使用的:总是有一个问题，即 Windows 称你的 USB 转串行适配器是什么 COM 端口，或者在 Linux/OS X 中它是什么 TTY 设备

[Avishay]对这个问题有一个非常非常酷的解决方案:[在 USB 到串行转换器上放一个显示器](http://blog.avishorp.me/2012/12/wig2012-entry-xser.html)来告诉用户操作系统将其标记为哪个 COM 端口。

原型在 PIC 18F2553 开发板上运行。当插入 Windows 盒子时，串行适配器设置两个 USB 设备。第一个设备是一个[通信设备类](http://www.usb-software.org/usb_cdc.php)，它处理 USB 到串行连接的繁重工作。第二个 USB 设备是一个专有软件，它获取当前的 COM 端口号。由于 Windows PC 上的一个主机应用程序报告了串行适配器的 COM 端口，该数字显示在 LCD 上。

这是一种直到有人向你展示时你才知道你需要它的想法。来自[Avishay]的一个优秀的工具，虽然一对 7 段 led 灯可能会使它成为一个更具可制造性的设备。