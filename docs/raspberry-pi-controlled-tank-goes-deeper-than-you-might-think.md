# 树莓 Pi 控制的坦克比你想象的更深入

> 原文：<https://hackaday.com/2012/06/30/raspberry-pi-controlled-tank-goes-deeper-than-you-might-think/>

![](img/4948297f5da1b82cf1d19097d546f344.png "rpi-tank-hacking")

这个遥控坦克[现在接受树莓 Pi 板](http://blog.ianrenton.com/tag/raspberry-tank-build-diary/?order=asc)的命令。实际上，它接受通过 SSH 推送到 RPi 板的命令。这个控制方案效果很好。RPi 使用薄型 WiFi 转换器，在开机时自动连接到无线网络。这使得 SSH 进入设备变得轻而易举，一个更加用户友好的控制器将在未来的某个时候发挥作用。

但是真正重要的是让 RPi 与坦克的电路对话。仅仅是把恒隆虎 I 型遥控坦克拆开就被证明是一项繁重的工作，因为需要拆下踏板，而且要用很多螺丝把它固定在一起。不仅仅是替换所有的控制电路，【Ian】想要接入原来的控制器。为此，他花了一些时间用示波器分析信号，发现命令是以曼彻斯特编码格式发出的。他确定了各种数据包在做什么，使用晶体管保护电路板上的 GPIO 引脚，现在完全控制了坦克。硬件改造的最后一部分是用坦克的电池给 RPi 供电。

休息之后，你可以观看重新组装的坦克展示其新的无线控制器。

[http://www.youtube.com/watch?v=QSPcJL1CGjA](http://www.youtube.com/watch?v=QSPcJL1CGjA)