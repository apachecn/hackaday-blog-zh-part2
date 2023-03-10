# Arduino 云盾

> 原文：<https://hackaday.com/2014/08/05/the-arduino-yun-shield/>

![YUN](img/50da8ba8cfd91123d5a34dd19f9b5d3b.png)

几年前，将 Arduino 项目放到 web 上的最常见方法是添加一个加载了 OpenWrt 的小型路由器，连接一个串行连接，并将该路由器用作通往互联网的桥梁。这种奇怪的安排可能是因为现有的 Arduino 以太网和 WiFi 屏蔽太贵或功能不够，但不管怎样，Arduino 工作人员注意到了这一点，并发布了 Arduino Yun:一个带以太网端口的运行 Linux 的 SoC 的 Arduino。这就像一个 Arduino 连接到一个路由器上一样，额外的好处是拥有大量可用的库。

由于 Yun 基本上是一个嫁接到 Arduino 上的 SoC，我们很惊讶在之前我们没有见过[这样的东西。这是一个 Arduino shield，可以为从 Uno 到 Duemilanove 和 Mega 的任何 Arduino 板添加 Linux SoC、WiFi、以太网和 USB 主机。它与 Arduino Yun 基本相同，并且像 Yun 一样，它完全开放给任何人重新混合、共享和重用。](http://www.open-electronics.org/guest_projects/add-linux-wifi-ethernet-and-usb-to-arduino/)

在 Dragino 网站上找到的 Yun shield [具有一个运行 OpenWrt 的小型 SoC，通过串行连接与 Arduino 板的其余部分分离。该堆栈的 Linux 端具有 400MHz AR9331(与 Yun 相同的处理器)，16 MB 的闪存和 64 MB 的 RAM，用于运行内置的 web 服务器，并将 Arduino 可以收集的所有传感器数据发送到云(顺便说一下，Yun 是指云)。](http://www.dragino.com/products/yunshield/item/86-yun-shield.html)

所有的硬件文件[都可以在云盾回购](https://github.com/dragino/modules/tree/master/hardware/YunShield)上获得， [Dragino HE 模块](http://wiki.dragino.com/index.php?title=Dragino_HE)是最难获得的部分。