# 思考帽也是派对帽

> 原文：<https://hackaday.com/2012/11/05/thinking-cap-is-also-party-hat/>

[![](img/acd94d6666cde14616e3da032d4d27bc.png "Thinking Cap")](http://hackaday.com/?attachment_id=89511)

[思维帽](http://www.empiricalnerd.com/2012/11/the-thinking-cap/ "The Thinking Cap")是一块可佩戴的标牌，让你展示你的想法。这顶帽子使用一个连接到蓝牙无线电的 Teensy 2.0，允许佩戴者动态更新信息，让房间知道他们在那一刻的想法。

这个黑客是基于 [LPD8806](http://hackaday.com/tag/lpd8806/ "LPD8806") 控制的 led 灯条，这种灯条非常流行，可以给任何东西添加大量的 LED。有五个条带需要通过 SPI 来控制，但 Teensy 只有一个 SPI 外设。

这导致多路复用器的使用，以允许单独控制每个条带。hat 采用一种有趣的低成本方案，利用两个 744052 双通道 4 通道多路复用器和一个 7400 反相器来多路复用五个通道。

青少年可以使用蓝牙串口协议接收信息。5 x 7 像素的字符存储在帧缓冲区中，并在帽子周围移动以创建动画。

结果是一个明亮的信息在用户的脑海中盘旋，可以通过蓝牙用智能手机更新。休息之后，请观看帽子的视频演示。

[https://www.youtube.com/embed/deTM_vJO1X0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/deTM_vJO1X0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)