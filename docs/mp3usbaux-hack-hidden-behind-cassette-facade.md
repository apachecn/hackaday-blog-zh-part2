# 隐藏在盒式磁带正面后面的 MP3/USB/Aux Hack

> 原文：<https://hackaday.com/2013/04/04/mp3usbaux-hack-hidden-behind-cassette-facade/>

![mp3-hiding-in-plain-sight](img/52052d916a760116ea1b4e2d2660d164.png)

[伊凡]用这个汽车音响系统做了些特别的东西。他把主机改成了从 USB 播放 MP3 文件，并增加了一个辅助线路。但是看着它你永远不会知道。这要感谢他所做的工作，创造了一个隐藏音频插孔的假按钮，以及一个隐藏 USB 端口和 MP3 播放器显示屏的假盒子。可能最好的部分是收音机本身仍然像以前一样工作。

有几个组成部分使这个系统运转起来。它从盒式磁带/收音机头单元开始。除此之外，他还在 Deal Extreme 上买了一个带遥控器的 MP3 播放器。他不太喜欢附带的红外遥控器，所以他在方向盘上安装了一个遥控器。为了将所有东西组合在一起，他使用了 PIC 16F877a。微控制器控制告知磁头单元磁带是否已插入的线路。当[Ivan]选择 Aux 输入或想要从拇指驱动器播放 MP3 时，uC 会强制主机进入盒式模式，播放器的音频会注入盒式播放器连接。

为了帮助阻止盗窃，[伊万]创造了两个虚假的战线。盒式磁带的一端插入 USB 端口。倒带按钮插入辅助插孔。休息之后，您可以在演示中好好看看这两者。

[https://www.youtube.com/embed/Yvaf-cADcNk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Yvaf-cADcNk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)