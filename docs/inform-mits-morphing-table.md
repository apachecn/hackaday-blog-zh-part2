# 告知:麻省理工学院的变形表

> 原文：<https://hackaday.com/2013/11/07/inform-mits-morphing-table/>

你曾经希望你的餐桌可以通过盐吗？麻省理工学院的进步可能很快使这成为现实——尽管它可能会把盐撒得到处都是。进入 [inFORM:通过形状和对象驱动的动态物理启示和约束。](http://tangible.media.mit.edu/project/inform/)

虽然麻省理工学院的论文没有深入硬件本身的细节，但有一些有趣的花絮解释了它是如何工作的。在一个 30 x 30 像素的阵列中，有 900 个单独驱动的白色聚苯乙烯引脚组成了该表面。高射投影仪提供系统的视觉引导。每个销可以驱动 100 毫米，每个销施加高达 1.08 [牛顿](http://en.wikipedia.org/wiki/Newton_(unit))的力。为了实现致动，使用推拉杆来最大化密集的引脚排列，如图所示，使得显示器与致动器的尺寸无关。驱动是通过使用由 ATMega2560s 驱动的定制 PCB 的 6 个一组的电动滑动电位计实现的——这允许执行机构本身有一个极好的 PID 反馈方法。在论文的第 8 页有一张整个系统的极好的图片，显示了建造的规模和复杂性。遗憾的是，它看起来不像是可以在家里轻松制造的东西，但是，嘿，我们希望有人能证明我们是错的！

休息后留下来看看这项迷人的技术在发挥作用。该视频是由一个随机的俄罗斯 YouTube 帐户发布的，我们无法找到它的原始来源，所以如果你可以，请在评论中告诉我们！

[https://www.youtube.com/embed/UFd6WsObOu4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UFd6WsObOu4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【谢谢弗雷德里克！]