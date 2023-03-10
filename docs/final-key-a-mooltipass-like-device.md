# 最后一个关键:一个类似 Mooltipass 的设备

> 原文：<https://hackaday.com/2014/01/21/final-key-a-mooltipass-like-device/>

[![](img/1390030dfd4d3f2406d6524ce580bba1.png)](http://hackaday.com/wp-content/uploads/2014/01/finalkey.jpg)

自从 Hackaday 社区开始开发我们的离线密码管理器 Mooltipass 以来，我们已经收到了几个类似的 tips 项目。最后一把钥匙可能是迄今为止看起来最专业的一把。与[的 Mooltipass](http://hackaday.com/tag/developed-on-hackaday/) 类似，它基于 Atmel ATMega32U4，但只包括一个按钮和一个 LED，所有这些都封装在 3D 打印的外壳中。

最终键通过 USB 连接到主机，并被枚举为复合通信设备/ HID 键盘，需要基于 windows 的设备安装驱动程序。AES-256 加密密码存储在设备上，只有在按下按钮并通过命令行界面显示正确的 256 位密码后才能访问。凭证管理和访问也是通过后者完成的。不幸的是，Arduino 源代码在[cyberstalker]的网站上找不到，所以如果你看到你想集成到 Mooltipass 中的有趣功能，你可以给我们的 [Google Group](https://groups.google.com/forum/?hl=en#!forum/mooltipass) 发送消息。