# 在制作 UNIX 时钟的过程中犯了一些错误

> 原文：<https://hackaday.com/2013/11/30/making-an-unix-clock-while-making-a-few-mistakes-along-the-way/>

[![unixclock](img/162404f85324bc8ca9ccda0dd0c8c971.png)](http://hackaday.com/wp-content/uploads/2013/11/unixclock.jpg)

有时候，我们认为容易设计的项目却是我们最终犯最多错误的项目。你在上图中看到的 [UNIX 时钟](http://fowkc.wordpress.com/2013/10/30/unix-clock/)就是这些项目中的一个。对于不知道的读者来说，UNIX 时间是从 1970 年 1 月 1 日 00:00 开始的秒数。[詹姆斯]设计的时钟基于 Arduino Pro 迷你板、存储时间的 RTC 芯片、定制的显示板和两个设置日期/时间的按钮。

[詹姆斯]犯的一个错误是，在实际选择他将使用的七段显示器之前，设计了将焊接七段显示器的电路板，因为他认为它们都是一样的。他最终得到的显示器具有不同的间距，需要不同的阳极电压，因此他必须在 PCB 上切割几条迹线，并添加另一个电源。(詹姆斯)也花了很长时间来移除他的黑客空间的激光没有穿透的部分。如果你是电子世界的新手，我们强烈建议你好好看看他非常详细的文章。

如果你觉得这个 Unix 时间显示太容易阅读，这里的[是一个更大的挑战](http://hackaday.com/2013/08/14/unreadable-binary-epoch-clock-is-unreadable/)。