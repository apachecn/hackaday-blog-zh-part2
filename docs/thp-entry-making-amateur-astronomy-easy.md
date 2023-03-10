# THP 参赛作品:让业余天文学变得容易

> 原文：<https://hackaday.com/2014/06/25/thp-entry-making-amateur-astronomy-easy/>

随着电子技术的出现，业余天文学变得前所未有的简单。自动指向任何天文物体方向的望远镜支架已经存在了几十年，如果你对让机器人做你的工作太酷了，可以在你的取景器范围的视野中画出 0.5，2 和 4 度直径的圆的 Telrad 设备。[【Christoph】的 explorad](http://hackaday.io/project/1052-explorad) 采用了 Telrad 的概念，并增加了一些更多的电子扭曲:它仍然显示视野圈，但增加了对来自定制望远镜支架、巨大数据库和一些传感器的有趣天文物体的突出显示。

到目前为止，对任何自制天文物体发现者来说，最大的挑战是找出观测者在哪里。[Cristoph]不仅需要考虑地球上的位置(GPS 有助于这一点)，还需要考虑北在哪里(电子罗盘)，望远镜指向哪里(双轴支架上的光学编码器)，还要考虑世界时和当前的恒星时。生活在一颗围绕太阳旋转的行星上会产生大量代码。

[star finder 目前的进展击败了所有的 star finder](http://hackaday.io/project/1052/log/3970-this-was-the-biggest-omg-that-works-so-far)是一段代码，它绘制了“telrad circles ”,并用一个小三角形为每片天空显示占位符。倾斜设备或转动方位角锅移动这些三角形并动态加载新的三角形。现在这个游戏的名字是一个天空物体数据库，包含了[克里斯托夫]想要查看的所有天文物体。