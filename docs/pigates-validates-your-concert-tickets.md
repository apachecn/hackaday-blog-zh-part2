# 海盗验证你的演唱会门票

> 原文：<https://hackaday.com/2014/06/15/pigates-validates-your-concert-tickets/>

![gatespi](img/9e25d1c035116c742b9325e13b8ea7ce.png)

[Seph]在一家处理音乐会和特殊活动票务的公司工作。他的主要任务之一是在活动现场门口检查假票。根据场地的不同，这可以是磁条、条形码或几种 RFID 中的一种。直到最近，配备 USB 读卡器的上网本才能完成这项任务。然而，上网本并不是一个很好的解决方案——它们很贵，相对脆弱，而且占据了更多不必要的空间。

[Seph]有一个更好的主意。他用树莓 Pi 创建了一个[门票验证系统。Pi 放在一个半透明的盒子里，里面有一个](http://imgur.com/gallery/Nb5kX) [PiGlow](http://shop.pimoroni.com/products/piglow) RGB LED 板。USB 阅读器(在这种情况下是条形码阅读器)插入 Pi 的一个 USB 端口。这些阅读器可以在几种模式下运行，包括键盘模拟，这是[Seph]选择的，因为它不需要任何驱动程序工作。

使用 PiGates 是如此简单，甚至一个鼓手都可以处理它。通常 Pi 发出蓝色的光。当一张票被扫描时，[Seph 的] python 脚本读取代码，并根据在线数据库进行验证。如果票证有效，Pi 将会发绿光。闪烁的红色发光二极管指示假票。

点击休息时间查看更多关于 PiGates 的信息。

(Seph 的)公司在阵亡将士纪念日周末的一次活动中测试了该系统。PiGates 取得了巨大的成功。他的公司现在正计划用 PiGates 系统替换他们所有的上网本。

![piglowAnimation](img/17a0024c09028349637b20c5cc7c6342.png)

如果你想了解更多关于 PiGates 的信息，请查看 Reddit 上的[Seph]主题。