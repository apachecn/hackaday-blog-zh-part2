# CAN 黑客:硬件

> 原文：<https://hackaday.com/2013/11/05/can-hacking-the-hardware/>

到目前为止，我们已经讨论了 CAN 、[车载网络](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/ "CAN Hacking: The In-vehicle Network")和 CAN 上使用的[协议的](http://hackaday.com/2013/10/29/can-hacking-protocols/ "CAN Hacking: Protocols")[基础知识。最后，我们将讨论 CAN 工具以及构建您自己的 CAN 硬件所需的器件。](http://hackaday.com/2013/10/21/can-hacking-introductions/ "CAN Hacking: Introductions")

## 接线

不幸的是，CAN 连接没有固定的标准。高速 CAN 最常见的连接器是 DE-9，CAN 引脚 7 为高电平，CAN 引脚 2 为低电平。然而，电缆会有所不同，而且许多是不兼容的。

CAN 需要端接，最好通过总线两端的 120 欧姆电阻端接。实际上，你可以在总线上贴一个 120 欧姆的电阻来处理端接。

## 工具

一个好的 CAN 工具可以让你发送和接收 CAN 消息，使用 CAN 数据库解释实时数据，并讨论 CAN 协议。具有这一特性集的工具是专有的且昂贵的，但是存在一些黑客友好的选项。

### GoodThopter

[![The GoodThopter12](img/7aa1cd6fba1cbacccde790328fa3d7af.png)](http://hackaday.com/2013/11/05/can-hacking-the-hardware/goodthopter/)

基于[Travis Goodspeed 的] GoodFET，by [Q]的 [GoodThopter](http://goodfet.sourceforge.net/hardware/goodthopter12/ "GoodThopter12") 使用[微芯片 MCP2515](http://www.microchip.com/wwwproducts/Devices.aspx?dDocName=en010406 "MCP2515") CAN 到 SPI 控制器访问总线。开放硬件工具允许您使用 Python 脚本发送和接收消息。

### CAN 总线三重

[![CAN Bus Triple](img/d3ac8d5b1d7ddec8b583bd2419ed321d.png)](http://hackaday.com/2013/11/05/can-hacking-the-hardware/canbustriple/)

[CAN 总线三路](http://www.canb.us/ "CAN Bus Triple")器件提供了三条 CAN 总线的接口，可以在类似 Arduino 的环境中编程。提供的开源代码让你可以摆弄第二代马自达 3。不幸的是，硬件似乎不是开源的。

### 萨莱亚逻辑

[![Saleae Logic](img/bd34b6a8b11401603a403814dc426f17.png)](http://hackaday.com/2013/11/05/can-hacking-the-hardware/saleaelogic/)

它不是开源的，但是 Saleae 逻辑是一个非常方便和便宜的工具来查看 CAN 总线。它可以捕获、解码和显示 can 流量。这在您构建自己的 CAN 硬件时最为有用。

## 自己动手

### 零件

如果你想为 CAN 设计自己的硬件，你需要两样东西:一个 CAN 控制器和一个 CAN 收发器。

CAN 控制器生成并解释 CAN 消息。市场上有许多内置 CAN 控制器的微控制器，如 [Atmel ATmega32M1](http://www.atmel.com/devices/atmega32m1.aspx) 、 [Freescale S08D](http://www.freescale.com/webapp/sps/site/prod_summary.jsp?code=S08D) 和 [TI Tiva C 系列](http://www.ti.com/lsds/ti/microcontroller/tiva_arm_cortex/c_series/overview.page)。使用内置 CAN 控制器时，您必须使用外部振荡器，内部振荡器对于高速 CAN 不够精确。如果您想在现有微控制器上添加 CAN，MCP2515 是一个选项。它是一个独立的 CAN 控制器，通过 SPI 进行通信。

收发器将信号从控制器转换到总线，再从总线转换到收发器。高速和低速 CAN 网络需要不同的收发器。[恩智浦 TJA1050](http://www.nxp.com/products/automotive/transceivers/can_transceivers/series/TJA1050.html)) 支持高速总线，Semi NCV7356 上的[支持低速单线总线。](http://www.onsemi.com/PowerSolutions/product.do?id=NCV7356))

### 开发板

有大量的开发板采用带 CAN 控制器的微控制器。Arduino Due 的 SAM3 处理器有一个控制器，但板上没有收发器。你可以拿起一个 can 总线盾，和[到期的 CAN 库](https://github.com/collin80/due_can "Due CAN")一起上手。

[ChipKIT Max32](http://www.digilentinc.com/Products/Detail.cfm?Prod=CHIPKIT-MAX32) 与 Due 类似。它有两个 CAN 控制器，但你需要提供外部收发器才能真正上总线。幸运的是有一个保护罩。ChipKIT 由福特的 [OpenXC 平台](http://openxcplatform.com)官方支持，所以你可以[抓取他们的固件](https://github.com/openxc/vi-firmware)。

我们对 CAN 黑客攻击的讨论到此结束。希望你现在已经准备好去尝试这个协议了。如果您有任何问题，[请在主题中注明“CAN Hacking ”,发送到我们的提示热线](http://hackaday.com/contact-hack-a-day/),我们会整理出一些答案。如果你喜欢这个系列，并想为下一组帖子提出一个主题，我们也很乐意听到！

## 可以黑客攻击

*   [介绍](http://hackaday.com/2013/10/21/can-hacking-introductions)
*   [车载网络](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/)
*   [CAN 协议](http://hackaday.com/2013/10/29/can-hacking-protocols/)
*   [建筑 CAN 硬件](http://hackaday.com/2013/11/05/can-hacking-the-hardware/)