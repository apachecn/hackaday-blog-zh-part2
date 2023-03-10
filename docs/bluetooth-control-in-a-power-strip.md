# 电源板中的蓝牙控制

> 原文：<https://hackaday.com/2012/08/28/bluetooth-control-in-a-power-strip/>

![](img/8a42542e59198198cbdc1d08c3a9c734.png "bluetooth-power-strip")

[曼苏尔]在他房间的天花板附近安装了一个陶瓷空间加热器。由于热量上升，这不是最好的设计。他升级到红外线加热器，效果更好，但是缺少他在旧设备上使用的定时功能。他的解决方案不仅仅是增加一个计时器。为了无线控制设备，他最终在电源板中内置了一个蓝牙模块。他最终失去了除了两个插座以外的所有插座，但是所有的东西都符合原来的情况，所以我们认为这是一个合理的权衡。

他在火线和零线上都使用继电器来切换两个插座。这些通过 MOSFETs 驱动，以保护控制电路板的 ATmega168。微控制器和蓝牙模块都需要一个稳压 DC 电源，所以他在组合中包括了一个变压器和稳压器。休息之后，你可以看到他用两盏灯来演示这个系统。甚至还有一个终端界面，让你通过发送适当的字符来选择不同的控制命令。这个接口使得编写脚本变得轻而易举。

至少这个插线板不会[窥探你](http://hackaday.com/2012/07/22/power-pwns-price-tag-is-as-dangerous-as-its-black-hat-uses/)。

[https://www.youtube.com/embed/zcymzCllrcs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zcymzCllrcs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)