# Fubarino 竞赛:系统重置时的闪屏

> 原文：<https://hackaday.com/2013/12/29/fubarino-contest-splash-screen-on-system-reset/>

![logo](img/dfab75860db515b45297019b7097a325.png)

这里有一个 Fubarino 竞赛的参赛作品，是给那些自制电脑迷的。[Danjovic] [修改了一个 NTSC/PAL 显示适配器](http://danjovic.blogspot.com.br/2013/12/hackaday-fubarino-contest.html)以在他的主板第一次启动时显示一个 ASCII 版本的 Hackaday 徽标。

该版本基于[【Daryl Rictor】的视频显示适配器](http://sbc.rictor.org/io/vid3.html)，旨在用于自制计算机、微处理器项目和任何其他需要 NTSC 或 PAL 视频显示的极简数字设置。这是一个非常简单的电路，由几个逻辑 ic 和一个 ATmega8 组成。

[Danjovic]用复活节彩蛋修改了这个视频显示适配器:如果 ATmega8 上的一个引脚在电路板通电时短路，一个整洁的 Hackaday 闪屏会显示几秒钟，然后回到闪烁光标的股票显示。[Dnajovic]在一个简短的 Python 脚本的帮助下转换了 ASCII Hackaday 徽标，并通过一个小的固件更改将其加载到 AVR 上。

下面是开机画面的视频。

* * *

这是 Fubarino 竞赛的参赛作品，有机会获得微芯片作为奖品提供的 20 块 [Fubarino SD 板中的一块。](http://www.microchip.com/stellent/idcplg?IdcService=SS_GET_PAGE&nodeId=1406&dDocName=en566210)

[https://www.youtube.com/embed/krbLvOqsel0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/krbLvOqsel0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)