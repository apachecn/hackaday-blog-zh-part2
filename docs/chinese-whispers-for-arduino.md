# Arduino 的中国耳语

> 原文：<https://hackaday.com/2015/03/30/chinese-whispers-for-arduino/>

中文耳语或电话游戏包括告诉一个人一句话，让那个人告诉另一个人同样的话，并继续下去，直到紫猴洗碗机。今年的 Arduino 日，[Mastro]和一群 Arduino 一起在 Crunchlab 闲逛。你用一堆 Arduinos 做什么？[带软件序列号](http://www.mastrogippo.it/2015/03/arduino-day-2015-telephone-game/)的电话。

这个游戏的设置非常简单——让一个 Arduino 充当主机，监听(硬件)串行端口上的位。这个 Arduino 然后通过软件串行端口将这些位发送到 Arduino 链，直到它最终循环到主设备。结果显示在终端上。

在这场电话游戏中，只有大约 12 个 Arduinos，[Mastro]确实出现了一些传输错误。这有点令人惊讶，因为代码仅以 1200 bps 的速度运行，但这个游戏的要点不是完全准确。

[https://www.youtube.com/embed/KN225SBiyVU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KN225SBiyVU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)