# 弗兰肯斯坦博士的无线 Xbox One 方向盘

> 原文：<https://hackaday.com/2014/03/31/dr-frankensteins-wireless-xbox-one-steering-wheel/>

![](img/6f4e64a2add215d5b7ce589b3d821cff.png)买个 Xbox One 手柄马上黑？这正是[缇恩]所做的，所以他可以[将其与 SRW-S1 方向盘](http://hackaday.io/post/690)合并。他喜欢赛车游戏，并为能玩 Forza 5 而激动不已。他已经有了方向盘，但严格来说它只是一个电脑外设。[缇恩]想要方向盘来控制转向、油门和刹车，并发现 XB1 控制器和 SRW-S1 都非常适合黑客。

对于转向，[蒂尼]取代了 SRW S1 的加速度计 XB1 的左操纵杆锅。他将 X 和 Y 连接到 Arduino Pro 上的模拟引脚。然后，他使用 DAC 将旋转角度映射到电压水平，并将其连接到 XB1 操纵杆输出。XB1 控制器使用霍尔效应传感器和触发器上的磁铁来控制气体和制动。他移除了这些，并把 SRW-S1 桨连接到它们的输出端，XB1 控制器还是一无所知。

他还装配了一个 3 点控制系统来控制灵敏度和校准角度:一个按钮用于切换菜单项，两个触摸模块用于增加和减少数值。他将这些连接到一个反馈接口上，这个接口是通过重复使用 SRW-S1 的 15 个 LED 灯条制成的。最后，他在外壳内为 XB1 的大型隆隆电机留出了空间，并能够在一些 3d 打印附件的帮助下将小型电机连接到油门和刹车踏板上。休息之后，看看这个令人敬畏的黑客行动。

[https://player.vimeo.com/video/89103053](https://player.vimeo.com/video/89103053)