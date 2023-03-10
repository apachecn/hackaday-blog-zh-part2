# 美丽的 Arduino 烟花控制器

> 原文：<https://hackaday.com/2015/08/17/beautiful-arduino-fireworks-controller/>

许多设计师都有创造不应该爆炸的东西的奢侈。这通常很容易。诀窍是设计应该爆炸的东西，然后绝对确保它们在正确的时间爆炸(而且只在正确的时间)。[JonBush]最近做了一个漂亮的基于 Arduino 的焰火控制器。说真的，这看起来像一部夏季大片中的电影道具，布鲁斯·威利斯(Bruce Willis)正在试图决定剪什么线。

[Jon]使用 mega 2560，因为他想直接从该设备执行 I/O。他的代码只占总程序存储的 8K，所以通过一些 I/O 扩展(如[移位寄存器](http://hackaday.com/2015/03/18/an-experiment-in-shift-registers-and-multiplexed-leds/))一个更小的芯片就可以完成这项工作。该设备最多可以控制 8 组烟花，使用物理 arm 键，并具有手持遥控器。它甚至聪明到可以感知点火器故障。

前面板是一件艺术品，包括由 Neopixel LEDs 制成的七段显示屏。整个东西都在一个防水的盒子里，并在几个关键区域使用了光学隔离。

烟花是危险的，所以我们可能设计了更多的电子安全功能。比如电源开关只中断接地。关闭时断开两个电池腿可能更安全，这将使短路难以意外地为设备供电。在爆炸的商业设备上，你可能会看到双重输入，因此卡住的开关会导致故障(也就是说，启动或点火需要一个开关触点接通，另一个断开)。产出也是如此。驱动两侧的点火继电器使得卡住的输出更难意外点火。尽管如此，使用这样的盒子可能比点燃的朋克更安全，所以对于这个应用程序来说，它可能足够安全。

在过去的中，我们已经在[中看到了很多](http://hackaday.com/2008/11/15/microcontroller-fireworks-launcher/)[焰火控制者](http://hackaday.com/2013/02/18/wireless-fireworks-controller-includes-several-safety-features/)，但是他们中很少人的身体看起来这么好。我们希望在明年夏天的某部电影中看到它的副本。

[https://www.youtube.com/embed/ZiSjJKiuXxg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZiSjJKiuXxg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)