# Raspberry Pi 有助于 2.4GHz 家庭自动化

> 原文：<https://hackaday.com/2013/05/30/raspberry-pi-helps-with-2-4ghz-home-automation/>

为了扩展家中射频设备的功能【卡勒·勒夫格伦】[将一个树莓皮变成了一个射频控制中枢](http://gizmosnack.blogspot.se/2013/05/raspberry-pi-nrf24l01-and-tcp.html)。我们过去看过他的一些家庭自动化作品。在他的媒体室里，他建造了[一个通用远程基站](http://hackaday.com/2013/03/21/remote-control-command-center-includes-rf-and-ir-functions/)，它使用了与这个项目相同的射频板。主要区别在于，之前他使用的是 AVR 微控制器，而这次他升级到了 Raspberry Pi 板。

RPi 带来了更多的东西。特别是脚本(其输出如上所示)和网络特性。他的无线电板是 nRF24L01，他通过 SPI 协议与之对话。Raspberry Pi 通过其 GPIO 头与 SPI 设备对话没有问题。[卡勒]只需要做一些设置来配置引脚模式。

Python 脚本允许他使用键盘发送命令，但这也可以自动化。将它与他编写的 TCP 服务器脚本结合起来，就可以实现多种配置，以便与任何工作在 2.4 GHz 频段的设备进行切换或通话。