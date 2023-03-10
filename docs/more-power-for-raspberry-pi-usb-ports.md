# 为 Raspberry Pi USB 端口提供更多电源

> 原文：<https://hackaday.com/2015/04/06/more-power-for-raspberry-pi-usb-ports/>

自从 Raspberry Pi 2 发布以来，每个构建 RetroPi 模拟器的人都有了四个 USB 端口。对于我们这些用 Pi 做有用的事情的人来说，这些端口有点贫血:你不能同时插入网络摄像头和 WiFi 模块而不遭受 CPU 断电。所有 USB 外设可以从 USB 端口获得的最大电流为 600mA。[通过更改/boot/config.txt 文件](http://www.raspberrypi.org/forums/viewtopic.php?p=594183#p594183)中的值，所有四个端口的电流限制可增加至 1.2A。

![Pisquare](img/9eecc96dab9dde20b9853d786543c8e1.png)

The yellow line traces the signal from the GPIO to the USB power switch.

因为 USB 电流限制是在软件中设置的，所以必须有一些硬件来完成实际工作。藏在 GPIO 头右侧下方的硬件就是这样做的。这是一个 [AP2253 限流电源开关](http://www.diodes.com/datasheets/AP255x.pdf) (PDF)，通过在芯片上的第 5 号引脚连接一个电阻来调节电流。

AP2253 上的引脚 5 连接到两个电阻。一个电阻直接连接到接地层，而另一个通过 FET 进行切换。该 FET 的栅极连接到另一个电阻，当 GPIO 引脚为高电平时，这些电阻并联。这意味着当 GPIO 引脚为高电平时，电阻减半，AP2253 中的限流电路加倍。

这种设置提供了一种相对简单的方式来增加 USB 端口的电流限制，因此它们可以提供 4x500mA，符合 USB 规范。AP2253 电源开关的限流可以通过单个电阻设置，范围从 10kΩ到 232kΩ。通过移除 R50 和 R4，并用 10kΩ电阻替换 R50，AP2253 交换机的限流将被设置为最大值 2.1A。除以 4，每个端口为 500mA，就像地球上的所有其他计算机一样。

Raspberry Pi 基金会将 USB 端口的电流限制设置得如此之低是有原因的。Pi 最初是用来运行微型 USB 手机充电器的。市面上没有多少手机充电器能提供比 1A 更多的电量，而 CPU 和相关外设将占据其中的一半。如果你要修改/boot/config.txt 文件，你需要一个强大的电源。增加 2A USB 端口的电流限制将需要更大、更强的供应。