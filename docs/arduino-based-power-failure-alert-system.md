# 基于 Arduino 的停电预警系统

> 原文：<https://hackaday.com/2013/11/17/arduino-based-power-failure-alert-system/>

![arduinoPowerFailBox](img/b6a7f8a25c4252f9dc025e5f960476f6.png)

当他父母的商店停电，毁坏了他们冰箱里的东西时，劳特迈赫迪开始着手建造一个定制的停电警报系统，以防止未来的灾难。虽然一些商业产品解决了这个问题，但[Lauters]决定以同样的成本建造自己的产品，同时集成特定的警报功能:在主电源故障时向预定义的联系人发送短信。

第一步是实现 Arduino Micro 和诺基亚手机之间的通信。他的诺基亚 3310 使用 [FBus 协议](http://en.wikipedia.org/wiki/FBus)，但是【Lauters】找不到 Arduino 库来使这项工作更容易。相反，他通过运行 Arduino Uno 作为一个简单的串行中继器，直接从计算机向手机发出命令，实现了基本的通信原型，并最终研究出如何从“duino”发送 SMS。[Lauters]然后把手机拆开，点击电源按钮来控制开/关状态。他还断开了手机的电池，并将其插入一个附加的 PCB。该系统采用市电供电，但在停电期间会切换到 1000mAH 9V 备用电池，记录时间并发送短信警报。当电力恢复时，第二条消息通知联系人。

前往[Lauters 的]项目博客获取原理图和照片，然后查看[他的 GitHub 获取源代码](http://github.com/mehdilauters/arduinoPowerFailureAlarm)。如果你想看其他短信黑客项目，可以看看类似的建筑[保持一个远程小屋温暖](http://hackaday.com/2013/09/25/arduino-based-temp-control-via-sms/)，或者[通过短信激活的便携式电源板](http://hackaday.com/2011/09/13/portable-power-strip-control-lights-and-appliances-using-sms/)。