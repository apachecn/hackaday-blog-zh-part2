# 使用 ESP8266 切换主电源

> 原文：<https://hackaday.com/2015/04/19/switch-mains-power-with-an-esp8266/>

在我们开始之前，我们必须先声明:处理电源电压是非常危险的。除非你有资格，否则不要这样做！你可能会烧掉你的房子。(不加柠檬。)也就是说，[TJ]已经创建了一个有趣的[开发板，用于通过现在无处不在的 ESP8266 模块控制 WiFi](http://www.esp8266-projects.com/2015/04/p2-wifi-web-power-switch-for-mains-mpsm.html) 上的电源电压。只有 50 毫米 x 25mm 毫米，很容易小到足以安装在接线盒内！

被称为 MPSMv2，该项目的核心是 ESP8266 模块。开发板本身可以支持任何带有 GPIO 引脚的产品，无论是 Arudino、Raspberry Pi 还是任何具有这些特性的产品。刷新 NodeMCU 固件几乎是让设备启动并运行所需要做的全部工作，一旦你将设备连接到你的 WiFi，你就可以控制你想要的任何设备。

该设备使用一个[三端双向可控硅开关](http://en.wikipedia.org/wiki/TRIAC)进行切换，并且与电源光学隔离。请务必在休息后观看视频，了解该设备的运行情况。总而言之，这可能是一个开始使用[家庭自动化](http://hackaday.com/2015/02/12/ridiculously-complicated-home-automation-made-simple/)的好方法，或者只是做一些简单的事情，比如为你的落地灯造一个[定时器](http://hackaday.com/2012/12/21/adding-a-timer-feature-to-this-desk-lamp/)。一切皆有可能！

[https://www.youtube.com/embed/nxnCAyv6qcw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nxnCAyv6qcw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)