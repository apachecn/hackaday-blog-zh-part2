# 用树莓派设计西蒙游戏

> 原文：<https://hackaday.com/2015/07/24/ddr-ing-a-simon-game-with-a-raspberry-pi/>

自 1998 年以来，我们有幸参与了一个名为 Dance Dance Revolution 的街机游戏，但在此之前，70 年代的西蒙游戏。它本质上是一个记忆游戏，要求玩家记住一系列的灯光和声音。[Uberdam]决定得到两个世界的最好的东西，并将两者混合在一起，创造了[这个巨大的脚控西蒙游戏](http://tixplicando.blogspot.com.br/2015/05/plataforma-simulate-com-raspberry.html)。([英译](https://translate.google.com/translate?sl=pt&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Ftixplicando.blogspot.com.br%2F2015%2F05%2Fplataforma-simulate-com-raspberry.html&edit-text=&act=url)。)

作为项目基础的木质平台安装了四个电容传感器，每个传感器代表西蒙游戏中的一种“颜色”。当玩家踩上一种颜色时，电容传感器会向继电器发送信号，继电器会依次通知树莓派大脑输入。Pi 还负责向玩家显示必须踩的彩色方块的顺序，并在投影仪上跟踪玩家的进度。

这是一个很好的方式，展示了像 Raspberry Pi 这样的小型计算机如何在利基环境中应用，同时也是一个非常有趣的游戏。我们都记得西蒙是令人沮丧的，我们只能想象在一个木箱上跳来跳去会使它更加令人兴奋。现在，谁能造出[一个能打败这个版本西蒙](http://hackaday.com/2014/06/09/beating-simon/)的机器人？

[https://www.youtube.com/embed/iasHndXMYgU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iasHndXMYgU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)