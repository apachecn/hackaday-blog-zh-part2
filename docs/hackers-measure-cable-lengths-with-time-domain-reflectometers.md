# 黑客用时域反射计测量电缆长度

> 原文：<https://hackaday.com/2015/07/27/hackers-measure-cable-lengths-with-time-domain-reflectometers/>

[android]已经为时域反射计(TDR)建立了一个[快速边沿脉冲发生器](http://www.eevblog.com/forum/projects/my-time-domain-reflectometer-%28a-la-w2aew%29/)。TDR 是一种简洁的技术，它让你[利用电信号](https://www.youtube.com/watch?v=Il_eju4D_TM)测量电缆长度，也可以用来定位电缆内部的故障。

TDR 的工作原理是通过电缆发送脉冲。当脉冲到达未端接电缆的末端时，它被反射回信号源。通过监测原始脉冲和其反射之间的延迟，可以确定电缆的长度。我们已经看到在之前使用 [TDR 的项目，它经常在电信行业用于定位长电缆线路中的故障。](http://hackaday.com/2015/04/14/projects-for-solving-big-water-problems/)

您可以在实验室中尝试 TDR，只使用示波器观察延迟，使用函数发生器产生脉冲。然而，这种技术对于上升时间非常快的脉冲效果更好。于是【android】基于[【w2 aw】s 设计](https://www.youtube.com/watch?v=9cP6w2odGUc)打造了一个快速边沿脉冲发生器。然后补充道，眼睛瞪得大大的。他的建造非常棒，是技术的一个很好的示范。