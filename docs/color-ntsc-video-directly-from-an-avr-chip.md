# 直接来自 AVR 芯片的彩色 NTSC 视频

> 原文：<https://hackaday.com/2013/03/27/color-ntsc-video-directly-from-an-avr-chip/>

![color-ntsc-from-avr-chip](img/fb58e18a6cef99fc65d6615796abcc4d.png)

我们以前已经多次看到 AVR 芯片输出的复合视频。但是我们不记得遇到过能够产生颜色信号的。这个项目就是这么做的，[从 ATmega168](http://www.youtube.com/watch?v=yhUCM9N-OKc) 产生一个彩色视频信号，而不使用外部集成电路。

[CNLohr]在这里展示他的成就。你会从他最近参与的载玻片 PCB 服务器项目中想起他。这一次是他正在开发的一个小游戏硬件。但使用微控制器的四个引脚，通过并联电阻连接，他能够产生彩色 NTSC 信号，而无需使用 AD723 等芯片。

休息后，你可以看到两分钟的演示，他展示了游戏运行一会儿，然后给出了一个信号是如何建立的概述。虽然没有太多的解释，但是他确实贴出了他的代码，也为你提供了一个自学 NTSC 标准的资源。也许可以做一个彩色版的[那个 AVR 的俄罗斯方块游戏](http://hackaday.com/2010/01/18/more-avr-tetris/)？

[https://www.youtube.com/embed/yhUCM9N-OKc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yhUCM9N-OKc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/electronics/comments/1az77m/color_ntsc_video_on_an_avr_without_an_ad723/)