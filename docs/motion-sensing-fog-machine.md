# 运动传感烟雾机

> 原文：<https://hackaday.com/2012/10/25/motion-sensing-fog-machine/>

![](img/b509209447a3a514553925a79033946f.png "Halloween")

我们最喜欢的节日就在眼前，所以看到一些吓唬孩子的小玩意出现在小费罐里也就不足为奇了。[Greg]也喜欢万圣节，显然表演得很好——他总是在万圣节前夕在门廊上使用一台造雾机，但在正确的时间触发它总是一件痛苦的事情。

今年，[格雷格]决定建造一台动作感应烟雾机。他的机器有一个有线遥控器，当制雾机准备好的时候有一个灯发出信号，还有一个按钮启动泵。这个遥控器在 120 伏交流电下运行，但[Greg]认为他可以在遥控器上插一个小型 USB 手机充电器，并为 ATtiny85 微控制器供电。

实际的电路只是一块 perfboard，一个来自 Sparkfun 的[大而旧的继电器，和一个去年捡回来的 PIR 传感器【Greg】。每当 PIR 检测到移动时，Tiny85 激活烟雾机 5 秒钟，并在 10 秒钟内解除警戒，直到再次检测到移动。这正是[格雷格]万圣节展示的互动氛围。](https://www.sparkfun.com/products/10733)

休息后的视频。

[https://www.youtube.com/embed/jfR2DZE90zY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jfR2DZE90zY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)