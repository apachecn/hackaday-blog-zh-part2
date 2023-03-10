# 用于平板游戏的无线弹球控制器

> 原文：<https://hackaday.com/2013/03/04/wireless-pinball-controller-for-tablet-gaming/>

![wireless-pinball-controller](img/bc4fb20a401db33711c9ccfe3cfbca81.png)

这个木头盒子是一个无线弹球控制器和平板电脑支架。这个想法是把它放在一个工作台上，给你一些站立和弹奏真品的快感。[Jeff]最近相当沉迷于在 Android 上玩弹球应用程序，并开始了这段旅程，因为他需要一种方式来缓解他的拇指。

Arduino 监控这个木制控制器两侧的按钮。[Jeff]是使用硬件的新手(他的职业是 Linux 内核开发人员),很快就遇到了按钮反跳问题。他选择了硬件解决方案，用两个与非门构建一个 SR 锁存器，而不是用软件来处理这个问题(我们在这个问题上有一个超级混乱的线程，我们最喜欢的线程在底部)。

随着输入的整理，他在项目中添加了一个 BlueSMiRF 板，使他能够通过蓝牙连接 Nexus 7 平板电脑。在这一点上，他遇到了一些问题，让设备响应他的控制，就像它是一个外部键盘。他的权宜之计是换一款不会抛出神秘错误的 Galaxy Tab 10.1。希望他会在下一次迭代中修复这个问题，这也将包括添加一个活塞来启动弹球，这是他写这个成功时刚刚收到的邮件中的一部分。

休息之后我们嵌入了他的快速演示视频。

[https://www.youtube.com/embed/R7NLa05LM5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/R7NLa05LM5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)