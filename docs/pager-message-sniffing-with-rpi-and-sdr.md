# 使用 RPi 和 SDR 嗅探寻呼机消息

> 原文：<https://hackaday.com/2013/06/18/pager-message-sniffing-with-rpi-and-sdr/>

![rpi-pager-message-sniffing](img/f5ba679c6e53a5ca1e3856836afa340b.png)

20 世纪 90 年代被称为，他们希望你使用现代技术来监听你朋友的寻呼机消息。说真的，现在有多少人还在用寻呼机？我们猜测你可以通过构建你自己的[软件定义的无线寻呼机消息解码器](http://www.raspberrypi.org/phpBB3/viewtopic.php?f=41&t=45142&p=357671)来找到答案。

[Sonny_Jim]买了一个基于 RTL2832 的 USB 加密狗来监听 [ADS-B](http://en.wikipedia.org/wiki/Automatic_dependent_surveillance-broadcast) 飞机通信，结果却发现该硬件无法在该带宽范围内进行通信。所以他开始寻找硬件适合的项目，并最终探索了寻呼设备使用的 POCSAG 协议[。原来它不仅仅用于人与人之间的交流。仍然有许多自动化系统使用这项技术。](http://en.wikipedia.org/wiki/POCSAG)

设置东西并不那么难。阅读项目日志上的评论显示有些人有依赖问题，但是这些听起来很平常，对你来说是一个复习 Linux-fu 的好机会。一旦所有的包都安装好了，你就可以简单地处理文本了，它可以以多种方式显示。[Sonny]在 Pi 的网络服务器上建立一个文本文件，这样他就可以从智能手机上查看最新的捕获。

[ [图像来源](http://commons.wikimedia.org/wiki/File:Pager_1.jpg "By Jakez (Own work) GFDL (http://www.gnu.org/copyleft/fdl.html) or CC-BY-SA-3.0 (http://creativecommons.org/licenses/by-sa/3.0), via Wikimedia Commons")