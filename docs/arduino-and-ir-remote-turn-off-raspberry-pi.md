# Arduino 和 IR 遥控器关闭 Raspberry Pi

> 原文：<https://hackaday.com/2015/07/18/arduino-and-ir-remote-turn-off-raspberry-pi/>

树莓 Pi 拥有所有很酷的功能，但它缺少一个电源按钮，这一点有些值得注意。在一个简单的设置中，切断微型计算机电源的唯一方法是物理地移除电源线。[Dalton63841]发现这低于他妻子对电子产品的耐受水平，[为他的树莓派](http://www.instructables.com/id/Turn-Raspberry-Pi-ON-w-Remote-Control/)做了一个简单的遥控器。

[Dalton63841]通过尝试使用 UART TX 引脚开始了这个项目，但结果是一个死胡同。他决定使用 Arduino 来监控 Pi 上的 3.3V 电源轨。当 Pi 在软件中关闭时，Arduino 可以感觉到 Pi 不再打开并断开电源。遥控器用于打开 Pi。Arduino 从遥控器读取 IR 代码，然后简单地给 Pi 加电。这是一个非常简单和优雅的解决方案，绝对不需要在 Raspberry Pi 上安装任何软件。

我们知道这不是我们曾经介绍过的技术上最复杂的项目，但是对于刚开始使用 Pi、Arduino 或 IR 的人来说，这是一个很好的初学者项目。此外，这可能是与[电池备份 Raspberry Pi 关闭设备](http://hackaday.com/2013/11/17/battery-backup-for-raspi-keeps-your-data-safe/)配对的最佳选择，该设备允许它在感知到断电时以可控的方式关闭电源。