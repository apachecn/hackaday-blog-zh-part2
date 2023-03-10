# 带 RPi 的机架式家庭自动化

> 原文：<https://hackaday.com/2013/02/06/rack-mount-home-automation-with-a-rpi/>

[![RPi Home Automation](img/e1e57d2c8d440a3025cc1a5df7495bfb.png)](http://hackaday.com/?attachment_id=94082)

[Patrick]想要对他房子的各个部分进行集中感应和控制。他的 [Raspberry Pi 家庭自动化系统](http://www.dumaisnet.ca/index.php?article=205f6247f86b88ae8941496569b5cd07 "RPi Home Automation System")在一个机架安装包中集成了一系列功能，这些功能是从一个旧的网络交换机中回收的。

自动化系统基于运行 Arch Linux 的 Raspberry Pi，它通过 SPI 与 ATmega 对话。我们已经多次看到这种设置用于向 Raspberry Pi 添加额外的端口，但使[Patrick]的构建与众不同的是他内置到系统中的控制量。

这个盒子控制日落和日出时的室外照明，产生唤醒电话，控制红外摄像机，并根据事件播放声音。它能够监测排水泵的水位，房子的报警状态，等等。自定义 REST API 用于与设备交互。这允许任何平台上的程序与他的家接口，并作为他家的 API。

[Patrick]在他的构建日志中提供了许多详细信息，这对任何想开发自己的家庭自动化系统的人都有帮助。还提供了来源。