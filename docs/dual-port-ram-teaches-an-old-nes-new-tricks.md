# 双口 RAM 教老 NES 新招

> 原文：<https://hackaday.com/2014/05/06/dual-port-ram-teaches-an-old-nes-new-tricks/>

![nesDPR](img/b88798c4131acbeff0738531f8f3c278.png)

[Andrew]正在为任天堂娱乐系统(NES)开发一款游戏。模拟器在这方面很棒，但是[安迪]喜欢在真正的铁上跑。为了提供帮助，他为他的 NES 设计了一个[双端口 RAM 接口。顾名思义，双端口 RAM 是一种带有两条独立的数据和地址总线的存储器。使用的](http://www.batslyadams.com/2014/05/nes-dual-port-ram-interface.html)[赛普拉斯半导体 CY7C136](http://www.cypress.com/?mpn=CY7C1360C-166AJXC) 【安迪】还包括仲裁逻辑，以确保两个端口不会试图访问同一个存储单元并导致数据损坏。在安迪的例子中，NES 在一边，没有注意到新的硬件。在双端口 RAM 的另一边，[Andy]安装了一个运行自己定制固件的 ATmega164。

新的硬件让[安迪]可以实时看到 NES 记忆中发生的事情。他添加了一个类似于 [FCEUX](http://www.fceux.com/web/home.html) 模拟器的实时内存查看/编辑屏幕。窗口在 PC 上运行，而游戏本身在 NES 上运行。[Andy]甚至能够通过将他的电路连接到 NES 的非屏蔽中断(NMI)线路来添加基本的中断和步进功能。通过保持 NMI 有效，ATmega 可以冻结正在进行的游戏。

[安迪]甚至用他的电路教 NES 一些新把戏。通过读取冰球上的计时器和得分记忆位置，他能够创建一个记分牌和球门灯。类似的技术被用于给魂斗罗一个枪口闪光，让[流光溢彩](http://hackaday.com/2013/08/05/no-computer-ambilight-clone-uses-a-computer/)系统相形见绌。

我们不知道[安迪]下一步计划是什么，但我们希望这是一个源代码发布，这样我们就可以自己动手破解一些游戏了！

点击休息时间观看几个[Andy 的] Vine 视频。

[https://vine.co/v/M6WzFBXeX1e/embed/simple](https://vine.co/v/M6WzFBXeX1e/embed/simple)

[https://vine.co/v/M6WZlFjdJ69/embed/simple](https://vine.co/v/M6WZlFjdJ69/embed/simple)