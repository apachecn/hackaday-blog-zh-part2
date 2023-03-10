# 投下阴影，弹奏音符

> 原文：<https://hackaday.com/2013/12/15/cast-a-shadow-play-a-note/>

![](img/b2c28c7907ba583c6f449d7cc91c2aa1.png)

想在这个假期寻找一种娱乐朋友和家人的方式吗？看看 Arduino 驱动的光电池钢琴就知道了。[Asahillis]发布了这个关于建造 6 音符音乐指挥中心的指令。

当演奏者把手放在钢琴上时，钢琴使用光敏电阻打开每个音符。音符可以使用盒子前面的电位计独立调音。黑客使用两个电路:一个产生音调，另一个混合它们。[Asahillis]改编了[[Forest Mims III]的](http://www.forrestmims.org/)永恒的原理图，用于 555 调音器和 741 混音器，以创建他的光电池钢琴。

当仪器通电时，代码读取环境光 5 秒钟，并根据其结果设置阈值。之后，第一个音符会响起，表明钢琴已经准备好演奏了。每个音符都有自己的 if-else 语句，告诉它在相应的光敏电阻达到低于设定阈值的值时发出声音(当玩家投下阴影时)。指南中有一个演示视频，但我们无法将其嵌入此处。休息过后，请观看演示视频。

如果你喜欢关灯摇滚，总有这款令人印象深刻的激光竖琴。

[https://www.youtube.com/embed/k2eS3LZmEzQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/k2eS3LZmEzQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)