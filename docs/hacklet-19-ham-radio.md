# hacklet 19–业余无线电

> 原文：<https://hackaday.com/2014/10/17/hacklet-19-ham-radio/>

![19](img/03cb2faa54cf9198e2d4791aa123bb8b.png)

业余或业余无线电操作员一直是黑客。在 20 世纪初的大部分时间里，买一台收音机很贵或者根本不可能。哈姆会建造他们自己的装备，一路上学习电子学和无线电理论。时间在流逝，但火腿们还在继续砍。今天我们在 [Hackaday.io](http://hackaday.io/) 上重点介绍一些最好的业余无线电项目！

[![rtl](img/647d0a932f960690f19f65ef8ce33209.png)](http://hackaday.io/project/3075)

我们从[DainBramage1991]和他的非常实用的 [RTL-SDR 开始，带上变频器和外壳](http://hackaday.io/project/3075)。[DainBramage1991]爱上了他的低成本 RTL 软件定义无线电加密狗。他甚至增加了一个简易的上变频器来覆盖高频波段。唯一的问题是射频噪声。Realtek 盘往往很少或没有过滤，这意味着它们非常容易受到噪声的影响。[DainBramage1991]使用了历史悠久的覆铜板绝缘技术。PCB 位固定 RTL-SDR 和上变频器。更多 PCB 将两块电路板分开。所有东西都放入一个钢制外壳中，将多余的射频拒之门外。

[![foxhunt-atten](img/e5ad2601d0e631bc57334cf838ab75ec.png)](http://hackaday.io/project/3075) 接下来是【瑞安米勒的又名 KG7HZQ】的[火腿电台猎狐衰减器](http://hackaday.io/project/2293)。火腿电台猎狐不包括吠叫狗或马。在这种情况下，猎狐是一场寻找隐藏的低功率发射机的比赛。如果你从未尝试过，那会很有趣。猎狐的挑战之一是当你非常接近时，找到发射机的方向。即使使用定向天线，反射和淹没的接收器也很难确定发射器的位置。解决方案是一个衰减器，它只是将信号降低到一个更合理的值。[Ryan]在他的电路中也使用了覆铜 PCB。由于衰减器器件直接焊接在 PCB 上，这更像是曼哈顿风格的设计。两个 1k 陶瓷锅帮助他实现了近乎完美的线性衰减目标。我们打赌这个衰减器将帮助[Ryan]赢得一些比赛！

[![psdr](img/6c93b915ad645acad467f212fcef72e2.png)](http://hackaday.io/project/1538) 谁说业余无线电不会带你去哪里？它很可能会把[迈克尔·R·科尔顿]带上太空！迈克尔的项目 [PortableSDR](http://hackaday.io/project/1538) 是黑客大奖[的五个决赛选手之一。我们在比赛的早些时候报道过迈克尔。PortableSDR 最初是一个业余无线电项目:一个便于业余爱好者在背包旅行中携带的无线电系统。它现在已经发展到如此之多，具有软件定义的无线电接收和传输、矢量网络分析、天线分析、GPS 和许多其他功能。我们非常喜欢[Michael]为瀑布显示、调谐和带通滤波器调整优化小型 LCD 的方式。](http://hackaday.io/prize)

[![e2ra](img/713fe0e64949334a395fe37f7d8e2c79.png)](http://hackaday.io/project/2507)【W5VO】正在做一个[以太网到无线电适配器](http://hackaday.io/project/2507)。无线电系统中的每一英尺同轴电缆都会丢失信号。人脉更差。所有这些加起来会造成几个 dB 的损失。[W5VO]希望在天线馈电点放置一个 SDR。随着信号路径的最小化，发射时更多的瓦特输出，收听时更多的信号回到接收器。SDR 和主机之间的接口将全部是数字的；准确地说是以太网。[W5VO]不是第一个这样做的人，微波系统多年来一直在天线处安装发射机和 LNB。这丝毫没有影响[W5VO]的设计。他已经安静了一段时间，但我们希望他继续他的设计！

其他人在哪里？本周我们的项目有点少，但我们有一个很好的理由。Hackaday.io 上没有足够的业余无线电项目！我们希望改变这种情况。你是业余无线电爱好者吗？在网站上记录你的项目。从其他火腿那里获得输入并推动信封！你甚至可能会发现自己在[火腿电台列表](http://hackaday.io/list/3188)！

这一集的黑客就讲到这里。和往常一样， [QRX](http://en.wikipedia.org/wiki/Q_code) 在下周。同样的黑客时间，同样的黑客频道，带给你最好的 [Hackaday.io](http://hackaday.io) ！ [73 年的！](http://en.wikipedia.org/wiki/92_Code)