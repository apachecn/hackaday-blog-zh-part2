# 单线设备网络

> 原文：<https://hackaday.com/2014/10/18/the-network-of-1-wire-devices/>

![teensynet](img/764b3d67249bd2e6549a9afc5de2ad6a.png)

[jimmayhugh]是一名家酿师，在他家周围有多个发酵室和储藏冷却器。他真幸运。然而，制造和储存啤酒的多种方法需要某种方式来告诉他的冷却器和发酵罐的温度。没有多少温度控制器可以监控两个以上的数字温度计或热电偶，[所以他想出了自己的](http://hackaday.io/project/693-teensynet)。它被称为 TeensyNet，它能够监视和控制多达 36 个 1 线设备，并将所有设备连接到他的家庭网络。

这个系统中的一切都使用[单总线协议](http://en.wikipedia.org/wiki/1-Wire)，这是一种由达拉斯半导体公司设计的总线，可以只用两条线连接设备；数据和地。(在*举行的*营销会议期间，我要做一只墙上的苍蝇……)【jimmay】正在使用[温度传感器](http://www.teensynet.com/teensynet-hardware/teensynet-ds18b20-digital-temperature-sensors/)、[数字开关](http://www.teensynet.com/teensynet-hardware/teensynet-ds2406-digital-switch/)、[热电偶](http://www.teensynet.com/teensynet-hardware/ds2762-k-type-thermocouple-sensor-board/)，甚至[一个图形 LCD](http://www.teensynet.com/teensynet-hardware/teensyglcd/) 和他的单线系统，一切都由一个 Teensy 3.1 和以太网模块控制，将一切都推送到他的网络。

所有设备都连接到网络后，[jimmay]可以进入他的个人 TeensyNet 网页，查看连接到任何网络控制器的所有设备的状态。这可能是达拉斯的工程师们做梦也想不到的，这是对家庭自动化未来的有趣展望，如果不是网络连接继电器的话。