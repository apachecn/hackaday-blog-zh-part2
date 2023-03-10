# 不可读的二进制纪元时钟不可读

> 原文：<https://hackaday.com/2013/08/14/unreadable-binary-epoch-clock-is-unreadable/>

![binary-epoch-clock](img/001bf4346b2e30c1ed975e22405c69ee.png)

现在几点了？就这件事而言，今天是几号？这只钟能告诉你这两件事，只要你能看懂它。这个二进制纪元工具包的灵感来自于一个[Maniaclal Labs]的朋友建造了一个 8 位二进制时钟。这是一个非常常见的项目，被重复用于像[电源定时逻辑驱动时钟](http://hackaday.com/2011/01/16/binary-clock-using-logic-chips-and-mains-frequency/)这样的事情。他们想为什么不把它做大呢？但是，即使这样，在研究了一点之后，你也能从这个展示中理解一些东西，你不会更接近于回答这两个问题。

问题是，这是不可读的在几个不同的方式。首先，你花了多长时间在脑子里算出上面显示的二进制数的十进制等效值？我们放弃了。但是把数字敲进谷歌(搜索十进制的:0b 0101001000001000001001010010010011)得到的是 1376260755。有意义？再说一次，不是对人类。这是 [Unix 时间](http://en.wikipedia.org/wiki/Unix_time)，这是从 Epoch: 8/11/13-22:39:15 开始经过的秒数。

看看下面的视频，展示如何设置时钟，它使用一个菜单系统进行人性化的输入。但由于它是 Arduino 兼容的，你也可以连接一根 FTDI 电缆，并在电脑上编程。哦，由于这是开源硬件(注意右下角的图标)，你可以从他们的 Github repo 中获得所有信息来构建(或试验板)你自己的硬件。

这是另一个复杂的时钟，它使用谢妮电子管显示时间和日期信息，这很有用。

[https://www.youtube.com/embed/zpKhnDOOV8o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zpKhnDOOV8o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)