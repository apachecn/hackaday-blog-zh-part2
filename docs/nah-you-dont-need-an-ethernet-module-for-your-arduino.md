# 不，你的 Arduino 不需要以太网模块

> 原文：<https://hackaday.com/2012/06/12/nah-you-dont-need-an-ethernet-module-for-your-arduino/>

![](img/d4661cf6961905ef4219042a9ac3d32d.png "wifi")

[Andy]需要一个数据收集 Arduino 和他的家庭服务器之间的廉价互联网连接。一个以太网屏蔽就足够了，但是他无法让 CAT5 找到 Arduino 的位置。无线屏蔽非常昂贵，在查看了流行的 Zigbee 模块后，[Andy]对范围和建造复杂性有一些担忧。

[解决这个问题的显而易见的方法](http://www.thebmwz3.co.uk/article.php?story=20120611144749730)是获得一个便宜的 WiFi 路由器，在设备上刷新 OpenWRT 固件，并通过 Arduino 的 USB 端口、路由器和 WiFi 连接将传感器数据传输到服务器。

[Andy]使用了易贝 15 号上的 TP-Link TL-WR703N 无线“旅行路由器”(我们检查时价格约为 30 美元)。在用 [OpenWRT](http://wiki.openwrt.org/toh/tp-link/tl-wr703n) 刷新路由器之后，【Andy】有了一个从远程数据收集 Arduino 直接到他的服务器的无线连接。

细心的 Hack a Day 读者会注意到这是本周第三个“无线路由器+ OpenWRT 作为开发板”的构建([第一个](http://hackaday.com/2012/06/10/using-a-router-as-a-wireless-embedded-platform/)，[第二个](http://hackaday.com/2012/06/11/adding-a-router-and-wireless-camera-to-a-remote-controlled-helicopter/))。不，我们不知道发生了什么，也不知道为什么全球制造商的集体无意识决定如此突然地锁定这种类型的构建。OpenWRT 可用于[数百种不同的路由器](http://wiki.openwrt.org/toh/start)，并且在我们的书中，任何使废弃路由器免于被填埋的东西(做一些有用的事情的好处)都是好的，所以如果你有另一个类似的构建，[在](http://hackaday.com/contact-hack-a-day/)中发送它，我们将在某个时间处理它。