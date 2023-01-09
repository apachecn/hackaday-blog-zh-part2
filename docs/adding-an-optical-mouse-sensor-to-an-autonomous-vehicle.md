# 给自动驾驶车辆添加光学鼠标传感器

> 原文：<https://hackaday.com/2013/04/03/adding-an-optical-mouse-sensor-to-an-autonomous-vehicle/>

[Tim]正在为 6 月 8 日 SparkFun 的 2013 年自动驾驶汽车比赛准备他的无人机。他有一个很好的开始，但在精确测量旅行距离方面有一些问题。他为这项任务选择的技术是将磁铁粘在车辆的轮轴上，并用霍尔效应传感器监控它们。这些传感器很挑剔，测试中的一些问题促使他考虑冗余系统。现在，他正在试验给自动驾驶汽车添加一个光学鼠标传感器。

最近，我们看到了同样的概念，但它是为了[跟踪全尺寸汽车](http://hackaday.com/2013/03/10/tracking-a-car-like-it-were-a-computer-mouse/)的运动。如果它能在那种应用中工作，它在这里应该是完美的，因为车辆更接近地面，并将在理想的条件下使用(天气晴朗的平坦路面)。[Tim]砸开了他放在周围的一个旧的惠普鼠标。在里面，他发现了一个阿瓦戈 ADNS-5020 传感器。拿到数据表后，他发现这只是一个 I2C 设备。上面你可以看到他用于第一次测试的 Arduino Leonardo。

[Tim]监控芯片的编码功能，包括一些有趣的功能，如测量传感器下方表面的对焦程度。这就带来了一个问题，在传感器无法准确报告之前，车辆的行驶速度是否有限制？