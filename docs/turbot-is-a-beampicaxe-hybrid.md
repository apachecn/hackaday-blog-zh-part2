# 多宝是一个梁/皮卡克斯杂交

> 原文：<https://hackaday.com/2013/10/13/turbot-is-a-beampicaxe-hybrid/>

[詹姆斯]想要建造一个梁大菱鲆。然而，他在光束电路方面遇到了一些问题，[最终得到了一个光束/Picaxe 混合](http://geppettosworkbench.blogspot.com/2013/10/beampicaxe-20x2-turbot.html)。 [光束机器人](http://en.wikipedia.org/wiki/BEAM_robotics)是[马克·蒂尔登](http://en.wikipedia.org/wiki/Mark_Tilden)的创意。首字母缩写代表生物学、电子学、美学和力学。在 20 世纪 90 年代和 21 世纪初，基于光束的机器人在爱好者中非常流行，但此后这种流行逐渐消失。光束机器人倾向于不使用微控制器，而是试图将事情简化到最少的元件数量。

【詹姆斯’】turbo 使用[米勒太阳能发动机](http://www.beam-wiki.org/wiki/Miller_Solar_Engine)。最初的设计是用发动机驱动一个[太阳能涡轮发动机](http://jwgoerlich.solarbotics.net/robots/scuff/circuit.htm)。[James']问题是机器人的光电二极管“眼睛”不能正确地使 74AC245 将电流传递给电机。由于机器人建造在一个狭小的空间里，调试电路极其困难。在与 245 奋斗了一段时间后，[James]决定为 Picaxe 微控制器更换光束电路。

Picaxe 每个引脚只能吸收或提供约 20ma 的电流，略低于[James']电机的空载电流。为了弥补这一点，他在每个电机上安装了四个引脚。发动机有引爆皮卡克斯的危险。然而，在轻载齿轮电机和低电流太阳能电池板之间，它似乎工作得很好。总的来说，该机器人是一个非常干净，紧凑的建设。跳过休息，检查其真正平稳的螃蟹般的行走动作。

[https://www.youtube.com/embed/Z99OIy8aJhI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Z99OIy8aJhI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)