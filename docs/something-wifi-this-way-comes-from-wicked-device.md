# WiFi 这样的东西来了；邪恶设备揭开野火面纱

> 原文：<https://hackaday.com/2013/11/28/something-wifi-this-way-comes-from-wicked-device/>

![WildFire-v2](img/a2bfa73eb6e69cbe35222094dcd10ac5.png)

Wicked Device 已经[向全世界发布了 WildFire 板](http://blog.wickeddevice.com/?p=494)。WildFire 是一个 Arduino 兼容处理器板，带有一个[德州仪器 CC3000](http://hackaday.com/2013/08/09/tiny-wifi-modules-again) 。WildFire 为典型的“杜伊诺克隆”添加了一些有趣的功能。WildFire 使用的不是 Arduino Uno 中使用的 ATMega328，而是 ATMega1284p，它提供 16K 的 SRAM 和 128K 的闪存 ROM(相比之下，Uno 中使用 2K RAM 和 32K 闪存)。板上还有一个微型 SD 卡插槽，用于数据记录功能。

在完全披露的名义下，我们应该提到[Adam]在 Wicked Device 认识[Victor 和 Ken]已经有几年了，并且得到了一个预发布版本的板来玩。与任何非标准 Arduino 板一样，WildFire 确实需要对 Arduino IDE 进行一些修改。这花了预发行版一些时间。从那以后，Wicked Device 简化了流程。一切都包含在他们的产品页面 的一个 [zip 文件中。一旦 IDE 启动并运行，很容易将 WildFire 的 CC3000 连接到您的本地接入点。从那里开始，互联网就是你的游乐场。对于那些已经在问“那么，黑客？”，请关注此空间——Adam 正在使用 WildFire 板进行黑客攻击，该板将在几天后发布。](http://wildfire.wickeddevice.com/)