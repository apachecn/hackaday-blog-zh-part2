# NES ROM 芯片嵌入板使盒式磁带可重新编程

> 原文：<https://hackaday.com/2012/06/15/drop-in-board-for-nes-rom-chip-makes-cartridge-reprogrammable/>

![](img/94cc40f1dcaa0a2e1af5ad6d3798a9a7.png "nes-flash-rom-replacement")

这里是来自[Dext0rb 的]超级任天堂弹夹的内脏。很容易就能挑出深色的板子，[让他通过 USB](http://electrifiedfoolingmachine.co/?page_id=633) 刷新 SNES rom。我们已经看到这样做了很多次，但这是一个比黑客们仅仅[添加一个死 bug 风格的内存芯片](http://hackaday.com/2011/04/12/play-unreleased-retro-games-on-the-real-thing/)更干净的选择。

他设计的电路板有一个双排引脚头，大小适合原始 ROM 芯片腾出的空间。该板有一个迷你 USB 连接器，可以通过他在盒式磁带外壳侧面切割的孔进行访问。这是在正确的地方，这样当它在 SNES 使用时你就不能把它插上(那会造成损坏)。ATmega32u4 芯片处理 USB 连接，并对存储 ROM 的 32 兆位闪存芯片进行编程。他在自己网站的博客部分发表了几篇文章，你会觉得很有趣。我们建议从[这个硬件玩笑话](http://electrifiedfoolingmachine.co/?p=571)开始。