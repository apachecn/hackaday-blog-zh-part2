# 时钟的轻度编程

> 原文：<https://hackaday.com/2012/05/08/light-programming-for-a-clock/>

![](img/7ba17c7b21b06cfa29235a37ed928816.png "light-programming-a-clock") +

所以乍一看，我们觉得这个钟没什么特别的。它基于 Arduino，使用字符 LCD 屏幕显示时间。但后来我们意识到，没有电池供电的 RTC，也没有按钮。你到底是怎么设定时间的？[Mossblaser]正在使用一个光编程器通过电脑屏幕设置时间。

我们以前尝试过几乎相同的数据传输技术，使用黑白闪烁的计算机屏幕[将曼彻斯特编码推送到光敏电阻](http://hackaday.com/2011/12/22/microcontroller-comm-with-a-computer-monitor/)。我们取得了有限的成功，但你可以看到[moss blaser]的钻机更加可靠，我们认为这背后有几个原因。首先，他每秒只发送 5 比特，这对于数字传输来说是非常慢的速度。这有助于弥补 LCD 屏幕刷新缓慢的问题。此外，LDR 被表壳背面的材料包围，这将有助于阻挡环境光。最后，他使用了屏幕的一小部分，而不是闪烁整个屏幕。这可以导致更精确的定时。你不得不承认，这很巧妙！

[https://www.youtube.com/embed/T5hS6n_OzEQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/T5hS6n_OzEQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)