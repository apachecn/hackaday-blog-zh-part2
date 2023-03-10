# 为损坏的除湿器控制器制造替代品

> 原文：<https://hackaday.com/2013/04/14/building-a-replacement-for-a-broken-dehumidifier-controller/>

![dehumidifier-replacement-controller](img/8ff57680c733c4b729a56e5a144a40d0.png)

我们曾想过自己做一个这样的项目，因为我们在网上订购的除湿机可以在任何湿度条件下全天候运转风扇。但这并不是说[大卫·吉罗尼]对他的设备的功能不满意。这是因为[除湿器控制器停止工作，所以他用自己设计的控制器](http://davidegironi.blogspot.it/2013/04/avr-atmega-dehumidifier-controller.html)取而代之。原来的湿度传感器是机械的，只是坏了。他使用 AVR 以及湿度和霜冻传感器让设备重新启动并运行。

ATmega8 芯片对 DHT22 湿度传感器进行轮询，并与用户可调节的 trimpot 值进行比较。如果高于该阈值，则使用上图中看到的继电器之一打开该装置。使用压缩机冷却设备时，你必须注意的一个问题是散热器上的积冰。[Davide]使用热敏电阻进行温度反馈，当温度低于 7 摄氏度时关闭压缩机，当温度高于 12 摄氏度时再次打开压缩机。

更换仍然使用储液罐传感器和指示灯。不过，我们建议使用芯片上的看门狗定时器，以确保在代码出错时复位。