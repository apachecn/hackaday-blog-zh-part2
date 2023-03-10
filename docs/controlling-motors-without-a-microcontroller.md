# 无微控制器控制电机

> 原文：<https://hackaday.com/2014/02/10/controlling-motors-without-a-microcontroller/>

![serial](img/15691567e3ed362f8f04772a3aa32dbc.png)

你认为你需要一个微控制器或者一个合适的电机驱动器来控制一个电机？不完全是。因为 RS-232 串口本身就是一个黑客，你可以只用一个串口和一个桥式驱动器来控制两个电机[。](http://www.instructables.com/id/How-to-Control-a-Motor-Through-a-Serial-Port-Witho/?ALLSTEPS)

该电路不使用串行端口上的数据引脚，而是使用 RS-232 接口的 DTR 和 RTS 控制信号。与串行端口的数据线不同，这些控制信号在使能时为高电平，并且还可以提供少量电流，足以控制 TA7291P 桥式驱动器上的一对引脚。

电路的其余部分由几个电阻和一对电机组成，软件只需打开和关闭 DTR 线和 RTS 线。一个小机器人摇摇摆摆地走过一张桌子就足够了，如果有正确的驱动程序，从废品抽屉里把零件拼凑起来就足够简单了。