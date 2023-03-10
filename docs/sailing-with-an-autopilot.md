# 用自动驾驶仪航行

> 原文：<https://hackaday.com/2013/11/12/sailing-with-an-autopilot/>

![sailboat](img/1787108f78c1c753f51ac402dcb2d7c2.png)

几天前看到皮划艇的自动驾驶仪后，[迈克]认为他应该提交他自己版本的水上自动驾驶仪。与适合单人皮划艇的东西相比，[迈克]的发明是一个巨大的装置，能够让一艘大型帆船保持恒定的航向。

为了跟踪船只的方位，[迈克]正在使用一个非常酷的数字罗盘，它使用发光二极管来保持稳定的航向。还包括一个令人惊讶的专业和非常昂贵的 6 轴 IMU。为了真正驾驶这艘船，[迈克]正在使用一个连接到舵柄上的线性致动器，由一个巨大的 60 安培电机控制器供电。该致动器仅消耗约 750 毫安，但如果[迈克]需要集装箱船或超级油轮的自动驾驶仪，电源就在那里。

为了控制，[Mike]最终使用了 Arduino、16 键键盘和 LCD 显示屏。通过这个，他可以将自动驾驶仪置于空闲、校准和运行模式，以及将船的航向向左或向右改变 1、10 和 100 度。

从一天的航行来看，[迈克]可以有把握地说他的自动驾驶仪工作得非常好。它能够保持顺风方向不变，甚至有足够的智慧逆风航行。

下面的视频。

[https://www.youtube.com/embed/FpBKKEKHAgY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FpBKKEKHAgY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/5SOgTuTnVS4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5SOgTuTnVS4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)