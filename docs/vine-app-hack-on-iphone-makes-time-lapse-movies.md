# IPhone 上的 Vine 应用程序 Hack 制作延时电影

> 原文：<https://hackaday.com/2013/05/22/vine-app-hack-on-iphone-makes-time-lapse-movies/>

![time-lapse-with-smashed-iphone](img/be9b2d7eaf1f0f37d8aee23a951a3a13.png)

Vine 应用程序最近风靡一时。它可以让你在 iPhone 上拍摄 6 秒钟的视频，并轻松地发布到互联网上。问题是[肖恩·哈金斯]没有发现时间限制对传统视频有用。但是如果你把它做成延时录像，你可以在 6 秒钟内塞进更多的信息。上面的装备是他对[的解决方案，让 Vine 应用程序充当延时记录器](http://www.idlehandsproject.com/?p=53)。

诀窍在于应用程序本身是如何工作的。它只在你触摸屏幕时录制视频。因此，你录制一秒钟的视频，然后移开手指，它会“暂停”录制，直到你准备好下一个场景。[Sean]通过添加一个伺服电机和一个触控笔来实现自动化。Arduino 驱动伺服系统，在屏幕上快速点击，在 6 秒钟内获得尽可能多的不同帧。起初，他在记录快速点击时有点困难。他的解决方案是将 3.3V 电压注入到他为该项目而拆除的触控笔中。点击上面的链接查看一些示例视频，或观看此嵌入式视频了解硬件的工作情况:

[https://www.youtube.com/embed/D0DI7plqEww?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/D0DI7plqEww?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)