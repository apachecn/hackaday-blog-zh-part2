# 黑客入侵 IPod 耳机控制器用于安卓系统

> 原文：<https://hackaday.com/2012/05/18/hacking-ipod-headphone-controller-for-use-with-android/>

![](img/1497ef14010e6fd0452e3d2a566f57cb.png "hacking-iPod-headphone-control-for-Android")

[Buddhra]想要使用一套耳塞，该耳塞还具有内置在电线中的控制器。他选择的耳机是为 iPod 准备的，但他认为它也可以用于 Android。他是对的，而且[设法改变了安卓使用的控制器](http://www.instructables.com/id/Galaxy-Nexus-and-others-headset-remote-with-medi),并且仍然把它放在原来的盒子里。

他已经做了一个定制的控制模块，具有快进和快退功能以及播放/暂停事件。用于控制的信号基于电阻分压器。iLuv 耳机上的播放/暂停按钮已经正常工作，所以他打开控制器，看看为什么前进和后退按钮不起作用。原来他所需要做的就是给那些按钮加上正确的电阻。在这里，你几乎可以看到 0603 表面贴装封装，他用来添加一个 220 欧姆电阻到后退按钮，和一个 600 欧姆电阻到前进开关。