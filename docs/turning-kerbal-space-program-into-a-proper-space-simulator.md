# 把 Kerbal 太空计划变成一个真正的太空模拟器

> 原文：<https://hackaday.com/2013/07/28/turning-kerbal-space-program-into-a-proper-space-simulator/>

![Kerbal](img/8e5fd391eb2bc5802a054519256915f4.png)

kerbal Space Program——一款由怪异的太空乐高和无能的小绿人组成的游戏——自从在 Steam 夏季大甩卖上推出以来，已经大受欢迎。现在，为了胜过那些在车库里建造 737 驾驶舱的飞行模拟迷，一些有事业心的 Kerbalnauts 正在为这个精彩的[齐奥尔科夫斯基]、[戈达德]和[埃维尔·金维尔]介绍建造定制控制器。

[vladoportos] [认为 KSP 可以使用定制的游戏控制器](http://forum.kerbalspaceprogram.com/showthread.php/42777-Custom-HW-gadget-Controller)来提供舞台、姿态保持和反应控制系统命令的开关。在游戏中，这些是通过键盘输入切换的，但不幸的是，这破坏了你的 Kerbal 志愿者成为火箭动力死亡天使的沉浸感。他装配了一个 Arduino Leonardo，每当他按下连接到他的试验板控制器的一个按钮时，就会向他的计算机发送 USB HID 命令。这是一项正在进行的工作，但[海参崴]有一些大的计划，包括一个物理导航球来显示他的船在空间的方向。

USB 输入是一回事，但这只是问题的一半。如果你想建造一个真正的 Kerbal 船模拟器，你需要从游戏的中获取数据*，并输入到你的眼镜或模拟显示器中。KSP 分部的[为你提供了解决方案](http://www.reddit.com/r/KerbalSpaceProgram/comments/1iri70/a_small_teaser_proto_still_a_lot_of_work_but_i/)。他一直在开发一个“任务控制”应用程序，该应用程序用 Python 运行，通过 TCP 连接到 Kerbal 空间程序插件，并显示飞行信息，如速度、高度、经度、纬度、远点和近点。代码就在[的 git](https://github.com/voneiden/ksp-missioncontrol) 上，准备好让某个人把它带到 Raspi 和字符 LCD 显示器上。*