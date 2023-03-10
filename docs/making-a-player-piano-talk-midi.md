# 让钢琴演奏者在 MIDI 上说话

> 原文：<https://hackaday.com/2014/12/25/making-a-player-piano-talk-midi/>

[Ramon]总是对钢琴着迷，当他在一家古董店偶然发现一些自动钢琴卷时，一个项目想法的小核心就形成了。他想知道是否有人曾经试图将一架演奏钢琴转换成一种完整的 MIDI 乐器，用计算机通过几个命令来拨动钢琴。这导致了我们所见过的最好的建筑之一:一架连接到电脑上的钢琴。

[Ramon]在 Craigslist 上花了几百美元找到了一架旧钢琴，一旦它进入工作室，拆卸就开始了。自动钢琴通过真空工作，空气通过风箱从钢琴卷上的几个小孔吸入。一系列通向每个键的管道将这些小孔翻译成音符。为 MIDI 设备复制这个系统是不可能的，但是有几家公司为演奏钢琴生产电子适配器。(雷蒙)所要做的就是复制这一点。

铅管被拆除，换上 88 个独立的电磁阀。这些阀门通过移位寄存器控制，移位寄存器由 ATMega 控制。在这个建筑中投入了惊人数量的电子和机械工作，成品显示了这一点。

好像把一架古老的钢琴变成一架能理解和演奏 MIDI 音乐的东西还不够，Ramon 决定在混音中加入一些视觉效果。他发现了一个比例为 16:4.5 的显示器——是的，有 16:9 的一半高——并将钢琴的前面变成了一个巨大的显示器。这十种不同风格的可视化是在处理过程中产生的。

![display](img/e7ff928ee3a0e2ee6b0f9de71ce1a303.png)

到目前为止，这架钢琴已经在奥克兰的一个互动艺术展上展出，希望它能参加明年的一个制造商博览会。也有计划让这架钢琴输出 MIDI，所有琴键下都有一个琴键扫描仪。令人印象深刻的工作。

下面视频。

[https://www.youtube.com/embed/vUkX8ig8D4A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vUkX8ig8D4A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)