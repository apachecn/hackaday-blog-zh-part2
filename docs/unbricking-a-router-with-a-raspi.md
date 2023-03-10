# 用锉刀拔出路由器

> 原文：<https://hackaday.com/2013/11/15/unbricking-a-router-with-a-raspi/>

大约十年前，[Mansour]了解到 Linksys WRT54G，这是一种无线路由器，几乎被应用到了世界上的每个项目中。在了解了这款设备的强大功能后，他决定进行固件升级。不幸的是，他不小心用砖头砸了这个路由器，让它在架子上放了几年。

闲置设备是魔鬼的玩物，当[Mansour]发现一个带 SDRAM 的三星硬盘与 WRT54G 兼容时，他决定尝试修复这个古老的路由器。只有一个问题:通过 JTAG 报头对路由器编程的最流行的实用程序需要一个 PC 并行端口。

[没问题，然后](http://blog.oxplot.com/debrick-wrt54gl-raspberrypi/)，因为【曼苏尔】手头有一个树莓派。并行端口实用程序把新的固件硬塞到路由器上，这是 Pi 上的 GPIO 端口绝对可以做到的。通过[向 debricking 实用程序添加 Pi 支持](https://github.com/oxplot/hairydairymaid-wrt54g-pi),【曼苏尔】只需要一点耐心和几根连接 GPIO 和 JTAG 接口的电线就有了一个功能正常的 WRT54G。