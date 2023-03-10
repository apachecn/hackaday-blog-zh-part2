# 六位数 VFD 闹钟

> 原文：<https://hackaday.com/2012/05/07/six-digit-vfd-alarm-clock/>

![](img/7d00f126eb55aeffb66439d0e86df9f8.png "vfd-tube-clock")

[Haris Andrianakis]刚刚完成[建造这个看起来非常干净的真空荧光显示时钟](http://www.candrian.gr/index.php/iv-11-vfd-tube-clock-final-design/)。它使用 IV-11 管显示六位数字，还有六个 RGB LEDs 来增加趣味(休息后看看视频中的例子)。ATmega168 驱动该设备，控制显示器并充当电池供电的实时时钟。

与任何电子管时钟一样，驱动显示器需要做大量的工作。每个灯管有一根灯丝，需要 1.2 伏电压，而灯管本身需要 60 伏电压才能点亮。微控制器不难保护；这是通过一系列基于晶体管的开关电路来实现的。但是需要三个电压(给微控制器、灯丝和分段供电)意味着更复杂的 PSU 设计。[Haris]选择使用 MAX6921 来简化过程。

如果你正在考虑建立这样的东西，我们建议寻找一些 12 段管。正如我们之前看到的，[它们可以显示字母和数字](http://hackaday.com/2011/02/25/a-vfd-clock-that-tells-the-time-then-tells-you-to-off/)，以防你希望在未来重新使用该设备。

[http://www.youtube.com/watch?v=wNwm_BL8msI](http://www.youtube.com/watch?v=wNwm_BL8msI)