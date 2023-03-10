# 将 Famicom 音频频道添加到 NES，而不会搞乱控制台

> 原文：<https://hackaday.com/2012/09/22/adding-famicom-audio-channles-to-an-nes-without-messing-up-the-console/>

![](img/709257ed73d1135c96999feac2d524e3.png "CastlevaniaIIImod")

[Callan Brown]来信向我们展示了一个非常有趣的 NES 音频黑客。[Callen]决定他想要完整的恶魔城 III 音频体验，这(没有修改)只能通过原来的日本 Famicom 控制台。[Callen]权衡了几个适配器选项后，决定推出自己的适配器。

问题是日本 Famicom 和美国 NES 实际上有不同的墨盒连接器。硬件从 60 针到 72 针连接器的变化增加了“功能”，如直接连接到扩展端口的 10 针(用于电视剧调制解调器之类的东西，谁知道呢)。另外两个额外的管脚被烦人的 [10NES](http://en.wikipedia.org/wiki/10NES) 锁定芯片使用。当他们这样做的时候，任天堂决定通过扩展连接器而不是盒式磁带来路由音频路径。

这意味着日本的墨盒不能管道声音到 NES 音频通道只有一个引脚适配器。好消息是，在找到隐藏在某些 NES 游戏(Stack Up，Gyromite)中的 pin 适配器后，音频可以很容易地从适配器 PCB 中取出。这需要更昂贵的 Famicom 恶魔城 III 墨盒(Akumajou Densetsu)。为了干净利落地把新的音频电缆从他的前端装载出来，NES(Callan)重新使用了牺牲适配器游戏的推车来制造某种邪恶的混合体。[Callan]还介绍了将翻译好的 ROM 闪存到日本游戏中的步骤。

多两个正方形和一个锯齿会有什么不同呢？来看看跳完之后的声音对比视频吧！谢谢[Callan]。

[https://www.youtube.com/embed/7v9339JUK3U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7v9339JUK3U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)