# 水箱液位计防止溢出

> 原文：<https://hackaday.com/2013/06/16/water-tank-level-meter-prevents-overflow/>

![roof-water-tank-level-meter](img/4d57feaf9e725a4e84bda2b2129d4d8f.png)

在[Raikut]居住的地区，大多数家庭的屋顶上都有水箱来装水。每一个都是用泵从井里注入的，重力是给家庭供水加压的一种方式。该系统不是自动的，需要房主手动开关水泵。[Raikut]通过设计一个 LED 条形指示器来监控水位，使这一过程变得更加容易。

传感器非常简单。每个 LED 基本上都有自己的电路，由一个晶体管和几个电阻控制。一个 5V 信号从 7805 线性调节器输入油箱。每个转换器的底部都连接到一根绝缘线，每根绝缘线在储罐中延伸不同的深度。当水上升时，它完成电路，点亮 LED。

[Raikut]具有节约意识，建造了一个蜂鸣器电路，它由指示最高水位的 LED 激活。如果有人在注水时离开水泵开关，当水到达顶部时，警报就会响起，他们可以在浪费水之前将其关闭。

[via [Reddit](http://www.reddit.com/r/electronics/comments/1g53id/sixpoint_water_level_indicator_for_tanks/)