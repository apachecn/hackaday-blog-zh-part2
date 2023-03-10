# 蓝牙步进电机驱动器

> 原文：<https://hackaday.com/2013/05/01/bluetooth-stepper-motor-driver/>

![bluetooth-stepper-motor-driver](img/c85db233f99d07bb9e08926ef95bc5ce.png)

[Dan]不久前从一台旧打印机上回收了一些零件，终于找到时间玩了玩。他最感兴趣的东西之一是上面看到的齿轮步进电机。他很快就能用 Arduino 让它运行起来，所以他决定把这个项目推进一点。他最终得到的是一个可以通过蓝牙控制的步进电机驱动器。

电机不能被直接驱动，但通过一个简单的电机驱动器，如[Dan]使用的 L293 芯片，不难将它们与您选择的控制硬件连接起来。从那里，他添加了一个 ATtiny85，它将负责移动电机所必需的步进协议。他使用的蓝牙模块作为一个串行设备，使得与 uC 的接口变得非常简单。[Dan]使用引脚接头来连接模块，因此将来切换到不同类型的串行设备将会快速而轻松。

休息之后，你可以看到他向驱动板发送步进命令。

[https://www.youtube.com/embed/oWj1sq8dN5w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oWj1sq8dN5w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)