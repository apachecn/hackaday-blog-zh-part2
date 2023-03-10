# 在树莓 PI 上获得低级 SPI 访问

> 原文：<https://hackaday.com/2012/07/27/gaining-low-level-spi-access-on-the-raspberry-pi/>

![Raspberry Pi - rpi](img/794e2a7cc7176c618443644fe411af74.png "raspi")

我们已经看到了大量将硬件与 Raspberry Pi 接口的项目。但它们通常依赖于钻头撞击。这意味着它们在软件中切换管脚以匹配特定的协议。事实是，支撑该板的结实的 Broadcom SoC 有许多内置外设，只是等待使用，而不是位碰撞。在这种情况下，可以通过用于 RPi 的 bcm2835 库访问硬件 SPI 外设。

真正使这一过程变得复杂的事情之一是 Broadcom 芯片和 RPi GPIO 接头之间的引脚映射。由于并非所有引脚都断开，所以 RPi 分线接头上的芯片中的所有 SPI0 引脚要么是运气好，要么是设计有远见。图书馆页面(上面的链接)很好地解释了这一点。但是，如果你正在寻找更多的工作示例，请查看[engineer bynight]的项目，其中[使用硬件 SPI](http://www.instructables.com/id/Preliminary-SPI-on-the-Pi-Communicating-with-a-) 添加了一个加速度计。