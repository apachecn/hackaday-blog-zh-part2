# 蓝牙网络监视器

> 原文：<https://hackaday.com/2013/01/11/bluetooth-network-monitor/>

[![Bluetooth Network Monitor](img/fe4f4378ddb6db2981e5a6e2177e38bf.png)](http://hackaday.com/?attachment_id=92890)

[Zak]想要监视他的网络连接，而不需要登录他的路由器。因为他的路由器是一台运行 Debian Linux 的个人电脑，他安装了一个蓝牙网络监视器来显示信息。

该监视器基于 ATMega328P，它从蓝牙串行连接中读取数据，并将其显示在 TFT 屏幕上。它使用低成本的蓝牙模块从路由器接收数据。shell 脚本获取数据，并将其格式化成可以通过蓝牙链路发送的字符串。

与台式电脑的 USB 连接用于为设备供电，但[Zak]还使用 [V-USB](http://www.obdev.at/products/vusb/index.html "V-USB") 添加了 USB 支持。他计划用它从桌面上获取数据。例如，他可以显示 CPU 负载和温度数据。

总的来说，这是一个无线获取数据并显示在桌面上的好项目。[Zak]提供了代码和他写的 Eagle 文件，供任何有兴趣构建它们的人使用。