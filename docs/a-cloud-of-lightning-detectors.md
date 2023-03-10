# 一群闪电探测器

> 原文：<https://hackaday.com/2014/06/29/a-cloud-of-lightning-detectors/>

![strikes](img/02101f29c94db36d39e1b65a97a36715.png)

这里有一个有趣的项目[来绘制地球上的每一次雷击](http://www.blitzortung.org/Webpages/index.php?lang=en&page=3)。Blitzortung 是一个使用许多极低成本的传感器板的项目，这些传感器板装有放大器、微控制器和以太网插座，用于检测雷击。当多个站点将所有的数据上传到服务器时，雷击的位置就可以被计算出来，即使它们离任何一个站点都有几百英里远。

每个站的工作原理都是利用大型环形天线或较小的铁氧体磁心天线来检测雷击引起的局部电磁场变化。这些信号可以被放大并转换成有用的数据，加上时间标记，然后在互联网上发送出去。从那里，这是一个简单的飞行时间计算，以精确定位闪电击中。

硬件实际上非常简单，基于 STM32F4 发现板。控制器包括以太网端口、GPS 单元、LCD 和所有与检测雷击相关的硬件。

如果你想看看一个连接到互联网的巨大闪电探测器网络的可能性，你可以查看一下 [LightningMaps](http://www.lightningmaps.org/realtime?lang=en) 看看有什么可能。

感谢[Sean]发送此邮件。