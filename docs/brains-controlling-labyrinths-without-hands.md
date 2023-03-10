# 大脑不用手控制迷宫

> 原文：<https://hackaday.com/2015/03/17/brains-controlling-labyrinths-without-hands/>

[Daniel]、[Gal]和[Maxim]上周末参加了一个黑客马拉松——braini hack 2015——在一天半的时间里，重点关注以神经科学为主题的构建。这三人是通信系统工程和计算机科学专业的学生，没有任何神经科学背景。你不可能在一天半的时间里造出一个 FMRI，所以他们最终凭借一款脑控迷宫游戏赢得了开源类别[的最佳项目。](http://harariprojects.com/2015/03/16/brainihack-2015-blue-gsd-with-brain-controlled-labyrinth-game/)

迷宫本身[完全是 3D 打印的](http://www.thingiverse.com/thing:725924)，比通常的“带孔的木制迷宫”简单得多，后者通常与迷宫谜题有关。它实际上只是一个让球跟随的塑料螺旋。这种简单是有原因的。该团队正在使用脑电图来检测脑电波，并在 X 轴和 Y 轴上移动迷宫。

该团队正在使用 [OpenBCI](http://www.openbci.com/) 作为他们大脑和一对伺服系统之间的接口。这实际上是一项有趣的技术。与一些玩具不同，如 [NeuroSky MindWave](http://hackaday.com/2012/12/20/modifying-an-eeg-headset-for-lucid-dreaming/) 和[星球大战力量训练器](http://hackaday.com/2015/02/22/use-the-force-luketo-turn-off-your-tv/)，OpenBCI 给你八个输入通道，可以连接到头皮上的任何地方。该团队使用这些输入来测量阿尔法波和稳态视觉诱发电位，以控制迷宫框架上的一对伺服系统。

这是一个伟大的构建，一个输出真实脑电图信号的设备的精彩演示，以及一个获奖的团队。不喜欢什么？