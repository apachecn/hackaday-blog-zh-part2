# 用 Mbed 控制铁路

> 原文：<https://hackaday.com/2013/08/14/controlling-a-railroad-with-an-mbed/>

![rr](img/ec884e07499d8e044757ab941149c019.png)

黑客这个词是从模型铁路俱乐部开始的，目前的技术水平掩盖了计算机控制和非常非常小的微控制器的进步。[Jim]用一个微控制器(在这种情况下是一个 ARM 供电的 mbed)制作了一个很棒的驾驶模型机车的教程。

低端模型机车由 DC 控制，因此 mbed 上的 H 桥和 PWM 输出有助于驱动这些列车。[Jim]连接一个 Pololu H 桥驱动器，连接到他的 mbed，一切运行良好。

铁轨道岔完全是另一回事。这些允许火车从一条轨道移动到另一条轨道，但是让它们向左或向右移动需要用 15 到 24 伏的高电流驱动螺线管。为此，[Jim]使用了一个 MOSFET 功率控制板来切换轨道，并制作了一个非常简洁的演示，展示了一个小型机车在一个轨道开关上来回移动。

还有另一类模型机车——采用数字命令控制的模型机车。这种设置只是一个安装在引擎内的小解码器芯片，它告诉机车打开灯或数字运行电机，允许列车员控制同一轨道上的多列火车。

[Jim]使用 mbed 讲解 DCC 的基础知识，允许两列火车使用计算机控制在铁路站场交换位置。这真的很酷，让我们想在地下室有更多的空间来开始建造一个巨大的计算机控制的模型铁路。

[https://www.youtube.com/embed/X6oJ_3nrTJ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/X6oJ_3nrTJ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/CMA0reXSTiM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CMA0reXSTiM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/2MC5PbsC9eE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2MC5PbsC9eE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)