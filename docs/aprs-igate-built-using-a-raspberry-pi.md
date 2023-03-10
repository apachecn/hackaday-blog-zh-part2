# APRS IGate 使用树莓 Pi 构建

> 原文：<https://hackaday.com/2012/10/19/aprs-igate-built-using-a-raspberry-pi/>

![](img/b342f615107a0ed1f346ed4e456b32ef.png "aprs-raspberry-pi")

上面看到的硬件用于[将本地射频无线电网络连接到 APRS-IS 网络](http://www.ultratechie.com/2012/10/pigate/)。APRS 信息系统是一种互联网服务，它使用网络连接在世界不同地方的 APRS 网络之间进行通信。Raspberry Pi 非常适合这个应用程序，因为它能够连接到网络，并且可以本地使用 Linux。

在软件方面，大部分工作是由 Python 脚本完成的。它负责建立和监控与 APRS 信息系统服务器的连接。为了连接到手持无线电单元，使用了 USB 声卡。 [Multimon](http://www.baycom.org/~tom/ham/linux/multimon.html) 包用于通过该硬件发送和接收音频包。

[Sunny]计划对系统进行一些升级。该设备需要向 APRS-IS 服务器报告其位置，并计划添加自动查找 WiFi 接入点位置的功能。也有可能完全去掉无线电，而[使用 DVB 加密狗作为软件定义的无线电](http://hackaday.com/2012/06/27/getting-started-with-software-defined-radio/)。