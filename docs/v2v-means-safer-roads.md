# V2V:汽车共享状态更新让通勤更安全

> 原文：<https://hackaday.com/2015/09/02/v2v-means-safer-roads/>

在美国，每年有超过 30，000 人死于车祸，还有更多人受伤。总的来说，人类不是好司机。在可靠的自动驾驶汽车进入全国各地的车库和车道之前，仍然有大量的工作可以做，以提高汽车的安全性，最大的希望是车辆对车辆的通信(V2V)。我们不断在新闻报道中听到这种技术，但基本技术几乎从未被讨论过。所以我决定看看在 V2V 早期我们可以期待什么样的硬件，以及当你的车开始与周围的其他车建立社交网络时你可以期待看到的功能。

### 这一切都开始于很久以前

V2V 通信的起源可以追溯到 1991 年，在名为《多式联运地面运输效率法案》(ISTEA)的法案中。ISTEA 最为人所知的是为 20 年后仍未建成的高速铁路线提供动力，以及要求 1998 年后销售的所有轿车和卡车安装安全气囊。ISTEA 还包括了一项名为自动公路系统项目(AHS)的研究条款，这项工作将为 V2V 通信奠定基础。

[![Image Credit: NIssan Motors](img/92938edf1d034ef110bc28fa4f79e1c1.png)](https://hackaday.com/wp-content/uploads/2015/08/thing.jpg)

Image Credit: Nissan Motors

AHS 项目的成果是圣地亚哥几英里的 I-15 公路被用作遥远未来技术的试验台。1997 年，自动公路演示开始，车辆配备了传感器、摄像头、油门、刹车和转向执行器、激光和毫米波测距仪，沿着一段嵌有磁性钉子的公路行驶。如果这个计划在整个美国实施，它将会非常昂贵，既要在所有高速公路上加装所需的传感器，又要在新车的价格上增加数千美元。然而，这是谷歌无人驾驶汽车概念的起源，以及未来十年将上路的所有无人驾驶汽车。

### 一个会说话的车队

AHS 项目展示了令人惊叹的技术，也是 V2V 通信的开端。在这个项目中，单个车辆可以加入一个“公路列车”，一个车队，每辆车一前一后，以减少风阻、阻力和燃料消耗。这是只有通过让计算机直接控制转向、油门和油门才有可能实现的事情，而目前 V2V 系统的提案并不是为这种情况设计的。

[https://www.youtube.com/embed/Dtj9J1A-PMk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Dtj9J1A-PMk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

2007 年，美国国家公路交通安全管理局(NHTSA) [发布了关于 V2V 通信未来的框架](http://www.regulations.gov/#!documentDetail;D=NHTSA-2014-0022-0179)，去年[发布了关于 V2V 技术](http://www.nhtsa.gov/staticfiles/rulemaking/pdf/V2V/Readiness-of-V2V-Technology-for-Application-812014.pdf)的准备就绪报告。这项技术还不可用，甚至 NHTSA 也要到明年才会发布规则制定的通知。该系统肯定会拯救生命，但它并不像自动驾驶汽车会让你相信的那样宏伟，也肯定不会兑现 20 年前的承诺。

### 无线网络

根据 NHTSA 准备报告，未来的 V2V 技术将在 5850 至 5925 MHz 频段中目前未使用的频率上进行通信。这仅高于目前用于 5GHz WiFi 的频带，当然，需要新的芯片、工具和协议。除了软件定义的无线电——而且是一个很好的——你将无法收听 V2V 通信。但是如果可以，你能看到什么？

[![Exploits, like [Charlie Miller]'s hack of the on-board entertainment system in a Jeep Cherokee presented at DEF CON this year, will hopefully be impossible through V2V communications](img/2ca207de6df1acfb76746fb391daf4ca.png)](https://hackaday.com/wp-content/uploads/2015/08/exploit.png) 

漏洞利用，像【查理·米勒】在今年的 DEF CON 上展示的吉普切诺基中对车载娱乐系统的黑客攻击，将有希望不可能通过 V2V 通信

当前对未来 V2V 协议的建议令人惊讶地面向安全性；毫无疑问，地方、州和联邦执法部门会喜欢一个能够不断广播高速公路上每辆车的速度以及车辆识别号的系统。很明显，这不会是一个受支持的特性。就目前情况来看，V2V 技术并不是对隐私的可怕侵犯；没有办法消除任何隐私风险，但拟议中的系统将至少与目前安装在汽车上的系统一样安全。

但是通过给汽车提供错误的信息来控制汽车呢？1997 年，一辆参与 AHS 计划的汽车将向后面的汽车传送有关其速度和即将遇到的障碍的信息。当然，在拟议的 V2V 系统下，有人可能足够聪明地欺骗尾随者的信息，让他们离开道路，对吗？

事实并非如此，也不是因为任何技术原因。出于责任原因，汽车制造商不愿意在油门、刹车和转向机构上安装任何执行器。汽车制造商似乎不想让持有 SDR 的人控制路上的大部分汽车。目前的建议是只向驾驶员显示*通知*，允许他们对即将到来的情况做出反应。V2V 不是一辆自动驾驶的汽车，但它可能会在未来被自动驾驶汽车使用。

V2V 离成为现实还有很长的路要走——最早，它可能会在未来几年出现在汽车上。这与 1997 年展示的技术相去甚远，但自动驾驶汽车正在迅速填补这一空白。这可能不会改变游戏规则，但 V2V 通信将大幅减少美国高速公路上的死亡人数，并有助于大幅减少事故数量。