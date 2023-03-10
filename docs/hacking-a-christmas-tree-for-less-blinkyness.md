# 砍一棵圣诞树以减少闪烁

> 原文：<https://hackaday.com/2013/12/27/hacking-a-christmas-tree-for-less-blinkyness/>

[![Hacking a Christmas Tree to Blink Slower](img/6312976e91ccb879dd2efe135fa8fae9.png)](http://hackaday.com/wp-content/uploads/2013/12/hacking-a-christmas-tree-to-blink-slower.jpg)

如果光纤自发光圣诞树闪得太快，会让你癫痫发作，那它还有什么用？如果你问[Mads Nielsen]又名[EcProjects]，答案是“不太好”。所以[EcProjects ]开始了一个小项目，将圣诞树的闪烁速度减慢到一个更合理的水平。这项任务起初似乎并不太难，但后来变成了构建变频 H 桥电机控制的优质教程。

打开树的底部后,[EcProjects]发现一个 12 伏的交流齿轮同步电机转动着一个多色半透明的塑料圆盘。一盏明亮的聚光灯透过转盘向上照进数百根小光纤的末端。当圆盘转动时，这种机制将大量的多色光从圣诞树树枝顶端的光纤末端排出。

他的目标是减慢马达的速度；然而，旋转是基于 50 赫兹的电源信号。为了继续使用这个电机，需要一个较低频率的交流电源。视频中接下来的内容是关于交流同步电机如何工作以及如何使用一些晶体管、电阻和 CMOS 4069 逆变器芯片构建变频控制和 H 桥的精彩课程。

最后，使用他的设计，在同步电机失速和反转之前，频率驱动只能降低到大约 30 Hz。[EcProjects]很大胆地列出了一些失败，这总是提供了更多的学习机会，非常值得赞赏。

如果你认为你有更好的解决方案，请在评论中分享你的想法。我敢肯定第一个提议将包括一个 Arduino 和[伺服修改为连续旋转](http://hackaday.com/2008/07/14/modifying-a-servo-for-continuous-rotation/)，但任何解决方案都将是迷人的，包括修改他的设计。休息之后你可以加入我们一起看视频。

[https://www.youtube.com/embed/ar6V-kFiwjI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ar6V-kFiwjI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)