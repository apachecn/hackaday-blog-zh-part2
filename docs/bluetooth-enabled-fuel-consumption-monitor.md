# 支持蓝牙的油耗监控器

> 原文：<https://hackaday.com/2015/01/09/bluetooth-enabled-fuel-consumption-monitor/>

[Malebuffy]去年给自己买了一艘二手船。他住的地方燃料并不便宜，所以他想要一种方法来监控他的燃料消耗。他最初考虑购买现成的 Flowscan，但它们太贵了。为了省钱，[Malebuffy]决定[开发自己的产品版本](http://malebuffy.blogspot.com/ "Bluetooth flow monitor")。

首先，[Malebuffy]知道他需要一种方法来显示收集到的燃料数据。他的船的控制台没有太多的空间，而且在他最近购买的船上打孔听起来不是个好主意。他决定用他的智能手机来显示数据。考虑到这一点，[Malebuffy]决定使用蓝牙将燃料传感器的数据传输到他的智能手机上。

该系统使用较旧的 Arduino 作为大脑。Arduino 从 05ZAT 燃油流量传感器的[微流中获取油耗读数。Arduino 处理数据，然后通过蓝牙模块将其传输到智能手机。整个电路由船上的电池通过 DC 适配器供电。电子设备被保护在一个防水的盒子里。](http://malebuffy.blogspot.com/2014/11/the-one.html "Fuel flow sensor")

[Malebuffy 的]定制安卓应用可以从他的网站下载。他还公开了 Arduino 代码，以防有人想要抄袭他的设计。