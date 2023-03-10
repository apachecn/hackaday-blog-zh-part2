# OpenPLC，用于万圣节展示的工业自动化

> 原文：<https://hackaday.com/2012/10/27/openplc-for-industrial-automation-to-halloween-displays/>

![](img/506a02dde567e7529aba5930da143d5c.png "board")

走出工厂的任何一个车间，你都会发现复杂的机器人正在建造任何可以想象的东西。这些机器需要以某种方式控制，在计算机时代之前，这些制造机器人是由继电器控制的，这些继电器连接在一起，产生大量的动作。继电器，不管有多可靠和防弹，如果不对整个机器重新布线，就不能被编程。现在，工厂有可编程逻辑控制器来处理他们的自动化任务。

【Thiago】[自建可编程逻辑控制器](http://code.google.com/p/open-plc/wiki/Main?tm=6)并作为开放硬件发布。OpenPLC 包括四个 24V 输入、四个 24V 输出(两个带 PWM)、0-10V 模拟输入以及用于编程和扩展的 USB、SPI 和 I2C。

如果你在车库里用工业机器制作任何东西，或者只是想要非常棒的万圣节(或圣诞节)装饰品，OpenPLC 可以负责驱动所有需要的螺线管、电机和致动器。通过可扩展的 I2C 和 SPI 总线，可以添加大量传感器，让项目变得生动。

OpenPLC 基于 ATMega328，与 Arduino 代码兼容。有一些用于数字和模拟 IO 以及以太网的扩展板。