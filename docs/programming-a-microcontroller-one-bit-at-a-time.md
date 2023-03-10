# 一次一位地对微控制器编程

> 原文：<https://hackaday.com/2012/09/24/programming-a-microcontroller-one-bit-at-a-time/>

![](img/e4a35520d9e7a81e50733a57fbd6a7c8.png "xkcd")

想象一下，你被困在一个荒岛上，离最近的人也有几百英里远，你终于有时间完成你正在做的项目了。你有一个微控制器，但你缺少一台计算机，你需要随时编程。你是怎么做到的？[androidruberoid]想出了如何使用三个开关和极大的耐心来手动刷新微控制器(俄语，出奇的好[翻译](http://translate.google.com/translate?sl=ru&tl=en&js=n&prev=_t&hl=ru&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fhabrahabr.ru%2Fpost%2F152052%2F&act=url))。

与几乎所有 Atmel 微控制器一样,[androidruberoid]的 ATtiny13 使用 SPI 接口进行编程。该接口需要四个信号:SCK、数据时钟、MOSI、从主机到从机的数据线、MISO、从机到主机的数据和复位。通过将这些数据线连接到按钮上，[androidruberoid]能够一次一个字节地手动键入新固件。

这种手动编程位的技术依赖于 SPI 接口没有最低速度这一事实。在休息后的视频中，可以看到【androidruberoid】用一个简单的程序手动编程了一个 ATtiny13。它只会点亮一个 LED，但如果有足够的耐心，他可以键入一个简单的“闪烁 LED”程序。

[https://www.youtube.com/embed/UJHeDvr_doM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UJHeDvr_doM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)