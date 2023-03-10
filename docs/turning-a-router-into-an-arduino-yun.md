# 将路由器变成 Arduino Yún

> 原文：<https://hackaday.com/2014/03/07/turning-a-router-into-an-arduino-yun/>

![yun](img/5a52d86db6c9091c727b03875f0296de.png)

Arduino Yún 是第一款新型 Arduinos，它在人们熟悉的 ATMega 微控制器和独特的引脚接头上增加了一个巨大的片上 Linux 系统。这是一个令人惊讶的强大系统，但也非常简单:基本上，它只是一个运行 Linux 的 Atheros AR9331，一个做 Arduino 事情的 ATMega32u4，两者通过串行连接相连。Atheros AR9931 也出现在硬件黑客流行的路由器中。有人将云软件移植到路由器上只是时间问题。

[Tony]拿了一个 TL-WR703N 路由器，装上 OpenWRT。把这个路由器变成一个 Yún 的 Linux 端是一件简单的事情，把 Yún 软件上传到路由器的根目录，然后重启它。Yún 的 Arduino 端由连接到路由器 USB 端口的 Arduino Mega 处理。快速更新 Arduino 的 boards.txt 文件，一个被黑在一起的 Yún 就差一条胶带了。

Yún 可能不是非常受欢迎，但它确实有一些有趣的用例。也许这还不足以让你在主板上花 70 美元，但是如果你已经有了一台 WR703 路由器，这是一个很好的实验方式。

谢谢[马特]的提示。