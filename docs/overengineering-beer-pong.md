# 过度工程啤酒乒乓

> 原文：<https://hackaday.com/2015/04/11/overengineering-beer-pong/>

如果有一个游戏值得用数百个发光二极管、传感器和电子模块进行过度设计，那就是啤酒乒乓。[杰夫] [创造了我们见过的最炫的啤酒乒乓桌](http://www.instructables.com/id/Interactive-LED-Beer-Pong-Table-20/?ALLSTEPS)。在一个巨大的 LED 显示屏上玩啤酒乒乓有点害羞，好家伙，看起来真不错。

桌子中央有一个 32×12 的 led 网格，桌子两端各有 10 个 Solo cups。这些豆荚每个都有 20 个 RGB LEDs 和红外传感器，可以对放在上面的杯子做出反应。桌子的外缘有 12 个供观众使用的 LED 环，使这款啤酒乒乓球桌在 608 个单独的频道上总共有 1122 个 LED。

这么多 led，如何驱动它们变得非常重要。这张桌子上有一个非常大的定制板，带有 PIC24 微控制器、TLC5955 PWM 驱动器和足够多的 IDC 接头，可以认真考虑使用 IDC 接头。

把足够多的发光二极管放在某个东西上，它肯定会很酷，但[Jeff]通过一些有趣的功能更进一步。有一个用电话控制桌子的蓝牙模块，一个给桌子一些基于音频的视觉效果的 VU 计，和清洁球的空气浴；把球扔进“进”洞，球会从“出”洞弹出，完好如初。如果你想知道做一张啤酒乒乓球桌要花多少力气，那就来吧。下面视频。

[https://www.youtube.com/embed/y7CqgSnP-7Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y7CqgSnP-7Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)