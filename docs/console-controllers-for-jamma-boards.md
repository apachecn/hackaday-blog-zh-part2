# JAMMA 板的控制台控制器

> 原文：<https://hackaday.com/2014/10/01/console-controllers-for-jamma-boards/>

在过去，我们指的是 80 年代末和 90 年代初，街机开始使用 JAMMA 标准，这是一种将单个街机板连接到控制器、视频输出和街机柜中其他昙花一现的设备的方法。从那时起，相当多的人已经收集了这些古董街机板。将它们投入使用需要一种提供电源、视频输出和控制器连接的方法。操纵杆和按钮的通常接线方式是用线束，但[迈克]和[王梓安]在树莓帽的帮助下将 Xbox 360 和 PS3 控制器连接到他们的机器[。](http://www.freecade.org/project-kajitsu/)

[迈克]和[王梓安]创建了项目 Kajitsu，以取代昂贵的“超级枪”控制器街机游戏收藏家通常用来玩街头霸王，x 战警和战斗蟾蜍。他们使用 Raspberry Pi B+上的 USB 端口来监听两个 XBox 或 PS3 控制器，并将按钮混合转换为这些旧游戏可以理解的内容。

这些人使用定制的 Linux 内核，只需几秒钟就能启动，提供最少的操作系统来支持控制器。棋盘本身极其简单；只有几个总线收发器、电容、电阻和接头。他们有一个 iPhone 质量的垂直视频概念验证视频(如下)，尽管他们仍在寻找简化蓝牙配对过程的最佳方式，[他们正在支持无线控制器的路上](http://www.freecade.org/project-kajitsu-bluetooth-proof-of-concept/)。

该板仅提供控制器输入。如果你有一个这样的旧主板，你将需要视频输出。那是另一个完全不同的项目，但是如果你有一个 SCART 监视器，那就非常简单。

[https://www.youtube.com/embed/ZyUOopUHAtk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZyUOopUHAtk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)