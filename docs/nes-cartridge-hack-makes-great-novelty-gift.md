# NES 墨盒黑客使伟大的新奇礼物

> 原文：<https://hackaday.com/2014/04/25/nes-cartridge-hack-makes-great-novelty-gift/>

![NES cartridge with arduino](img/c4db08307045c515c955f160f50c35bc.png)

我们大多数人都记得最初的 NES 系统上闪烁的死亡屏幕。这是由墨盒和 NES 墨盒连接器之间的不良连接引起的。不管出于什么原因，快速吹掉子弹成了一个非常流行的想法，尽管这并没有真正的帮助。[戴尔]决定通过制作 [NES 吹气车来解决这个烦人的问题！](http://facelesstech.wordpress.com/2014/04/25/nes-blow-cart/)

受之前[弹夹黑](http://hackaday.com/2014/01/28/the-8-bit-harmonica-blows-in-from-japan/)的启发，【戴尔】安装了一个定制电路，在超级马里奥/猎鸭弹夹中展示了曾经流行的 ATtiny85。一个小麦克风，连同开/关开关和程序头，放在原来的拾音器接口上。快速一击触发 ATtiny85 播放一首歌曲。

对[戴尔]来说，最困难的部分是弄清楚如何让它演奏“音乐”。随着名为 [Rtttl](http://en.wikipedia.org/wiki/Ring_Tone_Transfer_Language) 的库的发现，这个问题得到了解决。这使得他可以将老诺基亚的超级马里奥和塞尔达的铃声放到 Attiny85 上。包括 rtttl 库在内的所有文件都可以在他的 [github](https://github.com/facelessloser/Nes_blow_cart) 上获得。请务必在休息后留下来观看项目运行的视频。

[https://www.youtube.com/embed/QTKbzFRwih0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QTKbzFRwih0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)