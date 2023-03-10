# 修补 ODB II 和 CAN 总线

> 原文：<https://hackaday.com/2012/04/17/tinkering-with-odb-ii-and-the-can-bus/>

[Debrah]正在把他的下一个项目带到车库去。他使用 dsPIC 构建了自己的 CAN 总线阅读器。

使用控制局域网的好处是，它是每一辆现代生产线汽车的通用标准。正因为如此，使用该协议进行通信所需的芯片价格将超过一美元。[Debraj]选择了 MCP2551，它提供几种不同的 8 引脚封装。甚至还有针对 dsPIC33F 系列定制的应用笔记。

该项目采用 5V 和 3.3V 两种供电轨。这让事情变得有点复杂，但电平转换器可以确保芯片之间没有通信问题。一个四行字符的 LCD 在测试期间充当输出(你可以在休息后的剪辑中看到这一点)，但他已经有了第二个版本，在仪表板上看起来更好一些。

这个黑客还能做什么？嗯，我们之前已经见过[一种用于从方向盘](http://hackaday.com/2011/03/08/can-sniffing-for-steering-wheel-button-presses/)读取控制按钮的方法。这完全取决于你的车辆传输的是什么数据，找出答案的一种方法是建立一些硬件并开始记录数据包。http://www.youtube.com/watch?v=NHou_66MbgQT3