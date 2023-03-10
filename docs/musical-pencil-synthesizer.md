# 音乐铅笔合成器

> 原文：<https://hackaday.com/2013/09/29/musical-pencil-synthesizer/>

![ScreenShot031](img/0f2360168b006b61e9a7389b68d9b8df.png)

这是黑客幼徒的另一个有趣的周末项目，一个[音乐合成器](http://makezine.com/projects/drawdio-musical-pencil/)根据你的导电石墨绘图的电阻播放不同的音乐音调！

就像我们最近发布的关于 [DIY 金属探测器](http://hackaday.com/2013/09/28/diy-metal-detector/)的帖子一样，这个项目使用了曾经相关的 555 定时器。除了在这种情况下，他们使用更现代的 TLC555 定时器，只需要 3V，而不是典型的 4.5V。这是一个相当简单的项目，你应该能够在几个小时内完成。

电路很基本。555 定时器在非稳态模式下输出，这意味着有一个连续的脉冲流从引脚 3 直接进入扬声器电路。电路的其余部分监控铅笔接触的任何物体的电阻，包括你自己！电阻的变化导致 555 定时器输出脉冲的变化。

一如既往，视频指南在休息之后。

这项技术最酷的一点是你可以画不同的东西，包括钢琴，还可以用铅笔演奏音乐。因为你是阻力环的一部分，你可以有相当多的绘画乐趣！

[https://www.youtube.com/embed/P4-Wl0W1004?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/P4-Wl0W1004?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)