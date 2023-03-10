# Raspy 果汁给你串口和伺服控制

> 原文：<https://hackaday.com/2012/09/13/raspy-juice-gives-you-serial-ports-and-servo-control/>

![](img/3f8f4bf1307d3e40b9ae2de4d90c5daf.png "juice")

Raspberry Pi 扩展板的下一步是 [Raspy Juice](http://code.google.com/p/raspy-juice/) ，这是一种旨在将 Raspberry Pi 上的 GPIO 引脚分成伺服、串行和其他各种连接的板。

Raspy Juice 具有一个连接到 Raspberry Pi 的 ATMega168A 微控制器，作为 I2C 从设备。添加微控制器不仅为 Raspberry Pi 增加了模拟输入，还增加了 RS232 和 RS485 串行连接、实时时钟和四个用于业余爱好伺服的 JST 插头。

因为树莓 Pi 可以从 GPIO 头供电，所以创造者[NTT]增加了一个降压调节器，这样电池或太阳能电池就可以用来给树莓 Pi 供电。

Raspberry Pi 是一个非常棒的机器人平台，但遗憾的是，它受限于自身驱动电机和伺服系统的能力。Raspy Juice 为 Raspberry Pi 添加了一些急需的功能，我们迫不及待地想看到机器人通过这个扩展板迈出第一步。