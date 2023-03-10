# 任天堂 Power Pad 的第 14 款游戏

> 原文：<https://hackaday.com/2013/07/03/the-14th-game-for-the-nintendo-power-pad/>

[https://www.youtube.com/embed/6x23TWrInpI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6x23TWrInpI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

25 年前发布的任天堂 Power Pad 是一种插入 NES 的塑料垫，尽管在地下室和阁楼很流行，但成功非常有限。总共只有 6 款 Power Pad 游戏在北美发行，全球只有 13 款。cyborgDino 的人认为他们应该通过创建第 14 款游戏来庆祝 Power Pad [的银婚纪念日，使用 Arduino 并在 Unity 3D 中玩一会儿。](http://cyborgdino.com/2013/06/connecting-nes-power-pad-to-pc/)

第一项任务是读取电源板上的按钮输入。像所有 NES 外设一样，Power Pad 将其按钮的状态存储在移位寄存器中，可以通过 Arduino 轻松读取。在 UnoJoy 库的一点帮助下，让 Power Pad 按预期工作是一件相对简单的事情。

cyborgDino 创造的电子游戏叫做 Axis。有点像 Pong 和塔防游戏的交叉；把你的脚放在正确的按钮上，会弹出一个盾牌，保护你在屏幕中间的方块免受弹跳球的伤害。这是有史以来为 Power Pad 创作的第 14 款游戏，所以这肯定是有价值的。

下面的游戏视频。

[https://www.youtube.com/embed/Vn9moRgzrNo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Vn9moRgzrNo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)