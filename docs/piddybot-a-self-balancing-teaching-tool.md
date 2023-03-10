# PIDDYBOT——一个自我平衡的教学工具

> 原文：<https://hackaday.com/2014/01/17/piddybot-a-self-balancing-teaching-tool/>

[![](img/6ddac835d5b41ef9c87d81c15e369621.png)](http://hackaday.com/wp-content/uploads/2014/01/piddybottitle.jpg)

我们确信大多数 Hackaday 的读者已经熟悉了倒立摆系统，它基本上由一个重心在支点上方的摆组成。大多数应用(如我们将要描述的应用)通过将杆(或电路板)固定到旋转轴上将摆限制在 1 个自由度。因此，整个系统本质上是不稳定的，必须主动保持平衡以保持直立。

[肖恩]创造了 [piddybot](http://www.idlehandsproject.com/?p=267) ，一个微小的平衡机器人，旨在通过试图让机器人静止不动来教授 [PID 控制](http://en.wikipedia.org/wiki/PID_controller)的基础知识。更有趣的是，可以使用三个片上电位计直接调整比例/积分/微分值。这将允许用户感受每个参数对机器人行为的影响。piddybot 基于 Arduino nano，一个定制的 PCB，2 个 26:1 齿轮电机，一个 1A 双电机驱动板，一个六自由度[惯性测量单元](http://en.wikipedia.org/wiki/Inertial_measurement_unit)，2 块电池和最后一个 3D 打印体。休息之后，你可以看看机器人的视频。

这个项目源于[一个非 PID 自平衡器](http://hackaday.com/2013/09/26/self-balancing-arduino-does-it-without-an-imu/)，它是【Sean】在 9 月份一起黑出来的。

[https://www.youtube.com/embed/S9BQsCDw53s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/S9BQsCDw53s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)