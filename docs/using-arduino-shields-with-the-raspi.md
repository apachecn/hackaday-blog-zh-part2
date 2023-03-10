# 使用 Arduino 盾牌和 Raspi

> 原文：<https://hackaday.com/2012/10/10/using-arduino-shields-with-the-raspi/>

![](img/1146081c054ac5865e1e1113b4a81e34.png "aspi")

数百个 Arduino shields 可用于任何可以想象的应用程序，但很遗憾它们不能与 Raspberry Pi 一起使用。将 Raspi GPIO 引脚与 Arduino 兼容的接头分开，将允许制造商和修补者在更强大的计算平台上重复使用他们的屏蔽。

Cooking Hacks 的人意识到 Raspi 到 Arduino shield bridge 将是一个非常棒的设备，所以他们[制作了自己的](http://www.cooking-hacks.com/index.php/documentation/tutorials/raspberry-pi-to-arduino-shields-connection-bridge)，并配有一个软件库，允许你将 Arduino 代码直接移植到 Raspberry Pi。

Raspberry Pi 的 GPIO 头有一些限制；Raspi 没有模拟输入，所以 Cooking Hacks 团队增加了一个 8 通道 ADC。除了模拟输入和在板上弹出屏蔽所需的接头，还有一个 XBee 模块的插座。

软件库包含大多数通用 Arduino 功能，如 digitalWrite()和 digitalRead()。还实现了串行、有线和 SPI 库，允许任何通过 UART、I2C 或 SPI 通信的器件直接与 Raspberry Pi 对话。

虽然 Raspi Arduino 桥不允许与 Arduino 相同容量的 PWM，但您总是可以为这个整洁的小适配器提供伺服或 LED 屏蔽。