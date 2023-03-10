# CAN 黑客:车载网络

> 原文：<https://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/>

[上次](http://hackaday.com/2013/10/21/can-hacking-introductions/)，我们讨论了车载网络如何通过 CAN 工作。现在，我们将研究该协议及其在汽车行业中的应用。

## 公共汽车

在硬件方面，有两种类型的 CAN:差分(或高速)和单线。差分使用双线，工作速率最高可达 1 Mbps。单线在单线上运行，速度较低，但实施起来更便宜。差分用于更关键的应用，如发动机控制，单线用于不太重要的应用，如 HVAC 和窗户控制。

在多主机配置中，许多控制器可以连接到同一总线。所有消息都被广播到总线上的每个控制器。

[![An oversimplified in-vehicle network](img/f2b380e9f8125c905e2690cd40d4094b.png)](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/simple-car-network-2/)

An oversimplified in-vehicle network

[![The structure of a CAN message](img/dee94f4ed332444987ae19fbc83781ad.png)](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/can-message-structure-1/)

The structure of a CAN message

从软件角度来看，CAN 消息由 3 部分组成:标识符、数据长度代码和最多 8 个字节的数据。

标识符(ID)用于指定消息的含义和发送者。通常标准 id 是 11 位，但也有 29 位扩展类型 id。ID 还定义了优先级:ID 越低，消息的优先级越高。

数据长度代码(DLC)为 4 位，指定消息中有多少字节的数据。在某些应用中，DLC 始终为 8，未使用的数据字节用零填充。

最后，8 个字节的数据包含实际信息。信息的含义从信息 ID 中推断出来，长度由数据链路连接器指定。

## 解码和数据库

为了理解这 8 个数据字节，控制器会将数据解码成信号，如发动机转速、燃油油位或制动踏板位置。每个信号都有一个起始位和结束位，用于从 8 个字节中选择正确的位。没有信号信息通过总线传输。相反，所有管制员必须事先就信息和信号的布局达成一致。下面是信号表和示例消息的图形布局。

[![A table of CAN signals that make up a message](img/6dfed77bb250058f4bc9bf07b7b62abb.png)](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/can-table/)

A table of CAN signals that make up a message

[![](img/fba5b23d4635463d1d17494d86a5f4d8.png)](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/can-msg/)

A sample CAN message layout

为了帮助程序控制器在信息和信号上达成一致，使用了 CAN 数据库。该数据库包含所有消息和信号的定义。最流行的格式是 DBC，它是 Vector 的专有(但基于 ASCII)格式。DBC 编辑工具 [CANDB++](http://vector.com/vi_candb_en.html) 是免费的(就像在啤酒里一样)。数据库用于自动生成可以解释消息的代码。

有了数据库文件，您可以轻松地嗅探 can 总线并解释各种数据。一个例子是我们特别提到的一次黑客攻击，其中[嗅出了总线上方向盘按钮的按压](http://hackaday.com/2011/03/08/can-sniffing-for-steering-wheel-button-presses/)。您还可以通过向总线发送欺骗数据来伪装成控制器。例如，您可以向组合仪表发送一个假的发动机转速。

[![No, this car wasn't actually doing 8000 RPM.](img/2d9a017f64c47e783a424d12df3e2032.png)](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/fakerpm/)

No, this car wasn’t actually doing 8000 RPM.

正常操作期间的大多数通信都是通过解码数据库来完成的。但是，对于诊断应用，需要使用特殊的协议。下一次，我们将看看这些协议是如何工作的，以及它们能带来什么乐趣。

## 可以黑客攻击

*   [介绍](http://hackaday.com/2013/10/21/can-hacking-introductions)
*   [车载网络](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/)
*   [CAN 协议](http://hackaday.com/2013/10/29/can-hacking-protocols/)
*   [建筑 CAN 硬件](http://hackaday.com/2013/11/05/can-hacking-the-hardware/)