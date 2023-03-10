# 钟琴:吉他+钟琴混搭

> 原文：<https://hackaday.com/2012/11/28/glockentar-a-guitar-glockenspiel-mashup/>

[![](img/24d4b130eb9590a5560a507a178930c8.png "Glokentar")](http://hackaday.com/2012/11/28/glockentar-a-guitar-glockenspiel-mashup/glokentar/)

这种独特的电子乐器结合了切碎的吉他和劈开的钟琴以及 Arduino。[Aaron]的 [Glockentar](http://aaron-sherwood.com/works/glockentar/ "Glockentar") 由安装在木质机身上的吉他硬件和钟琴键组成。放置在琴键上方的螺线管驱动金属棒来演奏一个音符。

在引擎盖下，一个 Arduino 连接这些部件。导电拨片闭合电路，该电路是 Arduino 的数字输入。这就启动了相应的螺线管来演奏钟琴键，并通过串口向计算机发送字符。

在电脑上，一个基于[openframework](http://www.openframeworks.cc/ "openFrameworks")的程序创建灯光，投射到每根弦上。 [MadMapper](http://madmapper.com "MadMapper") 用于投影映射，将 openFrameworks 输出映射到每个字符串。视频使用 [Syphon](http://syphon.v002.info/) 框架在应用程序之间传递。

[Aaron]提供了一份深入细节的[报告](http://aaron-sherwood.com/blog/?p=381 "Glockentar Writeup")，包括该项目的 Arduino 和 openFrameworks 源代码。休息之后还有 Glockentar 的视频概述和演示。

[//player.vimeo.com/video/54077198](//player.vimeo.com/video/54077198)