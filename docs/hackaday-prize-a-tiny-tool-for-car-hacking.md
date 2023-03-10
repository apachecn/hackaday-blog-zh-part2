# 黑客日奖品入口:汽车黑客的小工具

> 原文：<https://hackaday.com/2015/08/10/hackaday-prize-a-tiny-tool-for-car-hacking/>

1940 年的汽车几乎完全是机械装置。然而现在，没有电的汽车是无法行驶的。不是引擎，而是电脑；汽车制造商希望不让我们这样的硬件黑客掌握其中的设计细节。[Mastro Gippo]想要构建一个小而强大的 CAN 总线逆向工程工具，而 [Crunchtrack 将其推出](https://hackaday.io/project/7134-crunchtrack)。它是一个 CAN 总线收发器、GPS 接收器和 GSM 调制解调器，所有这些都集成在一个小小的设备中，可以放在您的仪表板下。

[Mastro]对效率和微小的设备有轻微的迷恋，所以他将一切都打包在标准 ELM327 蓝牙适配器的外壳内。这是一个可以放在你手掌中的设备，但仍然可以(在计算机的帮助下)点击 can 总线，接收 GPS，并通过手机信号塔发送数据。

该设备基于 STM32 F3 ARM 微控制器(支持 mbed)、ublox 7 GPS 模块和 SIM800 GSM 模块，但故事并没有在硬件上停止。[Mastro]还在开发一个网站，汽车黑客可以在那里共享逆向工程数据。这使得这成为一个优秀的 Hackaday 奖项，我们迫不及待地想看看它从这里走向何方。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)