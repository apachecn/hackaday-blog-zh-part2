# 逆向工程司马 107 玩具直升机红外协议

> 原文：<https://hackaday.com/2012/08/27/reverse-engineering-a-syma-107-toy-helicopter-ir-protocol/>

![](img/627705389e2d78dd90e0e30fc8dbc2f6.png "reverse-engineering-IR-protocol")

给你的孩子买玩具的一半乐趣是当他们不再玩的时候，你能得到他们。[Kerry Wong]似乎在这条船上。他给儿子买了一架司马 S107G 直升机。飞行玩具是红外控制的，他逆向设计了它使用的协议。这不是我们第一次看到这种玩具。事实上，我们已经知道[协议已经被嗅到](http://hackaday.com/2012/03/23/decoding-then-cloning-an-ir-helicopter-toys-control-signals/)，甚至还有[一个干扰项目](http://hackaday.com/2012/01/26/jam-a-remote-helicopter/)在那里四处浮动。但我们对此进行了认真的研究，因为你可以从(克里的)过程中学到什么。

他首先将一个红外光电二极管连接到示波器上。这为他提供了命令之间的时序，并允许他验证信号是否编码在 38 kHz 载波信号中。然后，他切换到一个红外模块来解调这个频率。从那里，他捕获并绘制所有可能的控制配置，为设备建立时序和命令集。他基于 Arduino 构建了一个替换控制器，从而完成了这项工作。休息之后你可以看到那个硬件的视频。

[https://www.youtube.com/embed/dfY2OOQeogQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dfY2OOQeogQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)