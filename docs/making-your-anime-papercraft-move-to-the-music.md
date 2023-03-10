# 让你的动漫纸艺随着音乐而动

> 原文：<https://hackaday.com/2012/09/25/making-your-anime-papercraft-move-to-the-music/>

![](img/a98b10c600b76cccbd21c1ff78b248c0.png "anime-dances-to-the-music")

由于斯科特·哈登(Scott Harden)设计的一些电子动画技巧，这个动漫角色正在随着音乐起舞。她跳舞跳得很完美，在适当的时候展示不同的手臂和头部动作。同步的秘密实际上就在正在播放的音频的右声道中。

这个有争议的角色来自一个叫做 Leekspin song 的网络迷因。[斯科特]复制它在一些泡沫板上，增加一个伺服到一个手臂做韭菜旋转，另一个移动头部。这两辆车都是由 ATtiny44 驱动的。所有的动作都被预先设定好了，以配合音轨。但是他需要一种方法来同步每个动作集的开始。解决方案是用一个轨道对一组正弦波脉冲进行重新编码。右音频通道通过 LM741 运算放大器馈入 AVR 芯片。每个正弦波触发 AVR 执行序列中的下一个舞蹈动作。休息之后你可以看到这个项目的演示视频。

[https://www.youtube.com/embed/RzqdL5gqaHM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/RzqdL5gqaHM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)