# 用表演道具摧毁迪士尼的光芒

> 原文：<https://hackaday.com/2012/07/10/tearing-down-disneys-glow-with-the-show-props/>

![disneys-glow-with-the-show-teardown](img/32e1b7bfca21b09d54dd41d4c6edd2b2.png "disneys-glow-with-the-show-teardown")

安迪的老板最近刚从迪斯尼乐园回来，带着一副米老鼠耳朵。他说，活动中，人群中每一组“随秀发光”的耳朵都与表演同步变色。在他和一些同事推测这是如何实现的之后，[Andy 的]老板给了他一个新的任务——去发现这些该死的东西是如何工作的！

[安迪]小心地拆开耳朵，与我们分享他的发现和推测。在里面，他发现了一个由三节 AAA 电池供电的小型柔性电路板。该设备的中心是 TI MSP430G2553，其任务是控制嵌入耳朵的 RGB LEDs。

在一只耳朵里，他发现了他认为是 Vishay TSMP6000 红外接收器的东西。不管是不是 Vishay 品牌的，他用示波器和电视遥控器证实了它确实能接收到红外信号。在另一只耳朵里，他发现了一对小红外二极管，他推测这是用来重复在设备另一侧接收到的红外定时/同步信号。

同步方法似乎与我们前阵子讨论过的木管乐器完全不同，所以我们真的很想了解它们背后的技术。

留下来看看灯光秀的视频，因为[安迪]说他愿意接受任何关于迪士尼如何让他们的魔法发生的想法，请务必在评论中发表意见。

[https://www.youtube.com/embed/qVe93Vhbpxk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qVe93Vhbpxk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)