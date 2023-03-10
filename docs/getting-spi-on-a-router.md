# 在路由器上获取 SPI

> 原文：<https://hackaday.com/2013/08/17/getting-spi-on-a-router/>

![router](img/cb812027e140b360e5569ba39d8d4a7c.png)

像 TP-LINK 703n 和 TP-LINK MR3020(见上图)这样的廉价路由器不仅仅可以用来连接笔记本电脑和电缆调制解调器。它们实际上是非常小的 Linux 机器，通过 OpenWRT，你可以控制这些袖珍计算机的方方面面。人们经常认为，这些路由器是在微控制器上上网的常用方法的绝佳替代品，但你实际上是如何做到的呢？板载串行端口是一个很好的开始，但是这也会转储来自 Linux 控制台的输出。这里您需要的是 SPI 连接，而[ramcoderdude] [正好为您提供了解决方案](http://randomcoderdude.wordpress.com/2013/08/15/spi-over-gpio-in-openwrt/)。

Linux 已经有一些 SPI 模块，但是这些模块只能通过内核驱动程序访问。传统上，访问 SPI 的唯一方法是重新编译内核，但[coderdude]创建了一个内核模块，允许任何运行姿态调整 OpenWRT 映像的设备动态分配 SPI 总线。

他已经向 OpenWRT 开发者提交了这个补丁，希望它能包含在未来的更新中。我们认为这非常酷，它可以非常容易地为入侵路由器打开许多大门。