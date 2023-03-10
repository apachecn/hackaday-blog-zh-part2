# 中国 3020 数控机床获得一些升级

> 原文：<https://hackaday.com/2014/02/15/chinese-3020-cnc-machine-gets-some-upgrades/>

如果你经常去网上的 CNC 论坛，你会发现这些中国 3020 CNC 路由器普遍受到欢迎。人们普遍认为，控制电子设备还有待改进。[彼得]的感觉没有什么不同。他开始对他的机器的电子设备进行一些改进，例如[修复故障电源](http://lab.whitequark.org/notes/2014-02-11/cnc3020t-fixing-power-supply/)并增加 [PWM 主轴控制和限位开关](http://lab.whitequark.org/notes/2014-02-12/cnc3020t-emc2-configuration-and-hidden-features/)。

[Peter]确定电源中使用的变压器从次级线圈输出的电压超过了其他组件的处理能力。购买了两个开关模式电源，而不是用另一个变压器替换该变压器。一个给主轴供电，另一个给步进电机供电。所以他没有猜测电源所需的电流输出，[Peter]测量了步进机和主轴电机的运行电流。

收到后，主轴速度由控制面板上的电位计手动控制。数控机床控制软件，如 [LinuxCNC](http://www.linuxcnc.org) 或 [Mach3](http://www.machsupport.com/software/mach3/) ，具有使用 PWM 控制主轴速度的能力。原来，3020 的控制板和主轴电机驱动器就是为此而设计的，只是没有连接起来。在电路板上摸索一番后，完成这项工作所需要的只是添加两根跳线和拨动一个 DIP 开关。

控制板还有限位开关的输入，出厂时未使用。通过一些调查发现，限位开关输入是光隔离的。现在机器可以运行而不用担心无意中跑出行程。在[Peter]的网站上记录了这些内容，包括所有并行端口引脚功能和机器规格。

![3020lpt-input](img/f5fd03e4ba7707486e09c0ece7dea821.png)