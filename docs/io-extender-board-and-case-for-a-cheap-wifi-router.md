# 廉价 WiFi 路由器的 I/O 扩展板和外壳

> 原文：<https://hackaday.com/2012/06/24/io-extender-board-and-case-for-a-cheap-wifi-router/>

![](img/fc7e7ac8768ea89c5e82246ef2ec37b3.png "WR703N-io-extender")

这个 3d 打印的外壳容纳了已经很小的[TP-Link TL-WR703N],但也为定制扩展板腾出了空间。[扩展板的设计是为了让设备对黑客更友好](http://www.kean.com.au/oshw/WR703N/)，谁不需要[一个漂亮的外壳来装它](http://www.thingiverse.com/thing:25389)？

由于路由器板已经有一个 USB 端口(旨在与 USB 3G 调制解调器一起使用),该插件充当 USB 集线器。普通 USB 连接器被一个引脚接头取代，该引脚接头与扩展板下侧的 DIL 插座相匹配。通过使用 FTDI 芯片，扩展器提供了三个 USB 端口和一个 2×10 引脚接头，以将 GPIO 引脚从路由器处理器中分离出来。在上图中只能看到两个 USB 端口。那是因为第三个是凹进去的，外壳没有加开口。这让我们感到奇怪，直到我们了解到该端口是为了与一个低姿态的拇指驱动器一起使用，本质上是为该设备添加内部存储。

[谢谢巴斯]