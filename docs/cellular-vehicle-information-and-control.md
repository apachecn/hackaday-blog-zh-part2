# 蜂窝车辆信息和控制

> 原文：<https://hackaday.com/2012/10/13/cellular-vehicle-information-and-control/>

![](img/5f8ad0c82274ca89234e9ee3e1930a90.png "cellular-vehicle-control")

这个硬件是由[Bryon]和他的同学作为计算机工程项目建造的，它通过手机网络给你[反馈和控制汽车。它使用文本消息与控制设备通信。这几乎可以是任何手机，但在广告之后的剪辑中，他们展示了一个 Android 应用程序，它将一个漂亮的 GUI 放在你面前，并抽象出特殊格式信息的单调乏味。](http://www.bryonwheeler.com/2012/10/07/poor-mans-low-jack-using-arduino-and-cell-towers/)

该系统的核心是一个 Arduino Mega 板。它有一个带有外部天线的蜂窝屏蔽，用于连接。GPS 设备、中继板和 ODB-II 模块为系统提供反馈和控制。继电器允许汽车启动和车门上锁。GPS 和 ODB-II 模块可以发回位置和车辆信息(任何来自汽车传感器的信息)。在测试过程中，短信被屏蔽了，出现了一些问题。该小组认为，自动来回触发了某种来自电信的垃圾邮件过滤器。

如果他们真的想通过遥控驾驶汽车，还有很多工作要做。

[https://www.youtube.com/embed/jYkLBw-upYE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jYkLBw-upYE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)