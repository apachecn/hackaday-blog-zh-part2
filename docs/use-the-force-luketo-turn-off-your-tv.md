# 使用原力，卢克…关掉你的电视

> 原文：<https://hackaday.com/2015/02/22/use-the-force-luketo-turn-off-your-tv/>

你是否曾经光是想想就想打开或关闭电视？我们喜欢这个黑客主要是因为它使用了一个旧的星球大战[原力训练器](http://en.wikipedia.org/wiki/Force_Trainer)游戏。你仍然可以在网上花 40-80 美元买到它们。这个很酷的小玩具于 2009 年推出，使用一个带电极的耳机和一个脑电图(EEG)芯片。它传输脑电图数据来控制一个风扇，这个风扇向一个管子里吹气来“悬浮”一个球，同时由尤达的声音来指导。(Geesh！现在的孩子有最好的玩具！)

[Tinkernut]首先打开耳机，在那里他发现了一家名为 [NeuroSky](http://neurosky.com/biosensors/eeg-sensor/) (这是一家听起来很吓人的公司名称)的公司制造的脑电图芯片。PCB 设计师好心地在电路板上标记了 Tx/Rx 引脚，因此将它连接到 Arduino 上很容易。在从一台旧录像机中取出一个红外 LED 和接收器后，硬件就差不多完成了。经过一点编码，你现在可以使用原力控制你的电视！(好吧，我说的“力”是指脑电波。)休息后的视频。

注意:[Tinkernut 的] [博客页面](http://www.tinkernut.com/portfolio/homemade-mind-controlled-tv-remote/)应该很快会有更多信息。同时如果你能在 github 上找到他的 [Arduino 大脑库](https://github.com/kitschpatrol/brain/releases)。

这不是我们报道的第一个[脑电图到电视的接口](hackaday.com/2010/04/11/mind-controlled-tv/)。早在 2010 年，我们就推出了一个使用 Emotiv EPOC 脑电图耳机来开关电视的项目。但是 400 美元的耳机对普通绝地来说太贵了。

[https://www.youtube.com/embed/ThHrMW6Rtgg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ThHrMW6Rtgg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)