# Wide Word-clock 采用模块化方法

> 原文：<https://hackaday.com/2012/08/28/wide-word-clock-takes-a-modular-approach/>

![](img/c2b89cb07b1979f53c829897a825bec1.png "fat-word-clock")

[Ishan Karve]接受了建立自己的单词时钟的挑战。这是一个显示当前时间的时钟，如果有人问你现在是什么时间，你会使用相同的语法。你会发现周围有很多这样的项目，其中一个我们最喜欢的[使用蚀刻覆铜作为挡板](http://hackaday.com/2009/09/27/word-clock-tell-the-time-with-words/)。但是[伊山]打破常规，建造了一个长方形而不是正方形的钟。为此，他使用了由小模块组成的 16×8 LED 矩阵。

他设计了一个容纳 4×4 LED 矩阵的电路板，每个边缘都有引脚接头。这样，他可以将这些 16 像素的块排列成阵列，形成一个更大的网格。他用了八块木板做这座钟。它们由两个 MAX7219 芯片驱动，以 ATmega168 为主控制器，以 DS1307 计时。每个 LED 由一层厚的丙烯酸隔离，每个像素有一个孔。这可以防止光线渗入不应该照亮的字母。休息之后，请看片段中的结果。

[https://www.youtube.com/embed/UAORycrTEL0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UAORycrTEL0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)