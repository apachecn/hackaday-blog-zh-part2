# 实时探索 Mandelbrot 集

> 原文：<https://hackaday.com/2012/10/23/exploring-the-mandelbrot-set-in-real-time/>

![](img/0cfe0856060c2222a4b927d69f61acfd.png "brolt")

Mandelbrot 系列——如上图所示的分形“雪人翻身”——已经登上了杂志和期刊的封面，甚至已经在美术馆展出。对于一个只不过是数学函数的东西来说，这是一个令人印象深刻的壮举，并且已经成为[中岛千秋]痴迷的东西。

即使在现代计算机上，生成 Mandelbrot 集合的一部分的图像也要花相当多的时间。当[Chiaki]在 20 世纪 80 年代中期发现这种分形时，当时的计算机需要几个小时才能生成一张低分辨率的图像。实时缩放和滚动是不可能的，但[Chiaki]充分利用了他手头的东西，建造了 Pyxis，[一个完全由 TTL 逻辑芯片制成的 Mandelbrot 集生成器](http://www.chiaki.cc/Pyxis/index.htm)(谷歌翻译[这里](http://translate.google.com/translate?sl=ja&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fwww.chiaki.cc%2FPyxis%2Findex.htm&act=url))。

最初的 Pyxis 通过转接盒连接到台式电脑。而一个特殊的程序切换 Pyxis 内部的位和寄存器，生成 Mandelbrot 集合的图片，其速度比当时的 CPU 集合的速度快一千倍。

随着时间的推移，最初的逻辑芯片 Pyxis 很容易被最慢的上网本超越。然而，还有另一种方法来构建硬件 Mandelbrot 集生成器:FPGAs。

几年前，[Chiaki] [开始研究 Pyxis2010](http://www.chiaki.cc/Pyxis2010/index.htm) ( [翻译](http://www.chiaki.cc/Pyxis2010/index.htm))，这是一个基于 FPGA 的 Mandelbrot 集合生成器，能够动态缩放和平移世界上最流行的分形。[Chiaki]用 600 美元从 Digikey 买了一个 Altera Cyclone III FPGA(不，不是开发板，只是一个裸芯片)，开始把他的电路直接接到昂贵的 FPGA 引脚上[。一个手稳如泰山的男人，如果曾经有过恐惧的话。](http://www.chiaki.cc/Pyxis20img/pyxis2010-fpgasol2.jpg)

[Chiaki]没有将他的 Mandelbrot 发生器连接到计算机上并将其用作协处理器，而是决定要一种更便携的东西。他找到了一个旧的索尼 PSP，拆下了 LCD 屏幕，并将其集成到他的电路中。经过一点精心的设计和制作后，[Chiaki]有了一个手持的 Mandelbrot 生成器，它能够比任何台式计算机更快地显示世界上最著名的分形图像。

不言而喻，这个构建是不可思议的。在 FPGA 上构建一个速度惊人的 Mandelbrot 生成器的技术是惊人的，但是基于逻辑芯片的构建却是神圣的。休息之后，你可以看看这个令人惊叹的视频。

感谢[Ian Finder]将这封邮件发送进来。

[https://www.youtube.com/embed/aHp51yPUEaI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aHp51yPUEaI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)