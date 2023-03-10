# 4”七段显示器构成一个很好的记分牌

> 原文：<https://hackaday.com/2012/09/12/4-seven-segment-displays-make-a-fine-scoreboard/>

![](img/cea48d1ff4cb905758beb521db1e4ffe.png "simple-scoreboard")

[Blark]取了几个部分，[把它们变成了一个简单的记分牌](https://github.com/blark/Scoreboard/)。建筑的核心是一套 4 英寸的七段显示器。有了这些设备，只需要选择一个控制器向它们提供数据，并开发一个用户界面。

他似乎遇到了一些问题，因为他提到在焊接时炸毁了两个 PIC 芯片。他过渡到了 ATtiny24 芯片，现在一切似乎都很好。用户界面依赖于两个按钮，每个按钮增加一半显示的分数，同时按下两个按钮使游戏分数为零。显示器使用移位寄存器来存储数据，所以用 AVR 芯片很容易控制它们[。休息后请观看演示视频。](http://hackaday.com/2011/11/05/controlling-shift-registers-via-spi/)

这里唯一的问题是需要有人在场边来增加分数。我们已经看到了一些更复杂的设计，让你可以使用遥控器甚至智能手机。

[https://www.youtube.com/embed/6szSFfxwtfc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6szSFfxwtfc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)