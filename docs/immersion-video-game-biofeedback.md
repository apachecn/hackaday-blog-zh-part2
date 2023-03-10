# 沉浸式:视频游戏生物反馈

> 原文：<https://hackaday.com/2014/01/31/immersion-video-game-biofeedback/>

![immersionbiometrics](img/83b1cf40535c30758fd64441bfe39171.png)

我们不确定下面这个方法有多科学，但它确实很有趣。设计者[Samuel Matson]对游戏和压力之间的关系感兴趣，他拼凑了一个在游戏过程中提供生物反馈的设备。他参考了[this/r/gaming thread](http://www.reddit.com/r/gaming/comments/f8lev/)——在 Halo 会话期间测量玩家的心率——并进行自己的测试，监测游戏玩家的心率。几经反复，【Samuel】有了上图的耳机，它的特点是耳机旁边有一个熟悉的、可破解的[脉搏传感器](http://pulsesensor.myshopify.com/)。

该耳机使用 TinyDuino 和蓝牙 TinyShield 与玩家的计算机进行实时通信。然而，他并没有仅仅停留在监测心率上；他将信号整合到游戏设计中。[塞缪尔]使用 indie-favorite 游戏引擎 [Unity3d](http://unity3d.com/) 创建了一个第三人称射击游戏，当玩家心率增加时，它会通过提高难度级别来对脉搏传感器做出反应。他的目标似乎是减少或控制玩家之间的压力，但我们怀疑反转模型可能更有效:当你有压力时，让游戏让你放松一下，当你成熟时，给你一个挑战。

[谢谢肯]