# Arduino 转速表教程

> 原文：<https://hackaday.com/2012/08/30/arduino-tachometer-tutorial/>

![](img/385018ec8a07d37f44489f0a682128e6.png "arduino_tachometer_small")

本教程将指导您完成围绕 Arduino 构建转速表的过程。转速表用于测量转速，单位为每分钟转数(RPM)。你不需要太多的硬件，这个版本使用红外光束来测量风扇速度。和[去年基于 PIC 的教程](http://hackaday.com/2011/01/28/simple-sensors-to-calculate-rpm/)一样，【克里斯】使用字符 LCD 输出读数。LCD 的布线和驱动是最难的部分。

一对红外发射器/接收器位于风扇的两侧。当刀片从中间穿过时，接收器关闭连接到 Arduino 外部中断引脚之一的晶体管。他展示了如何使用这种中断来测量每个风扇叶片经过的时间。如果你除以叶片的数量，并平均读数以获得更高的精度，你可以很容易地计算出每分钟转数。

另一种选择是[使用反射传感器](http://hackaday.com/2011/04/22/simple-ir-bounce-tachometer/)，它允许发射器和接收器都在风扇的同一侧。