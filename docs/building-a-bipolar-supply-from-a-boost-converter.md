# 从升压转换器构建双极性电源

> 原文：<https://hackaday.com/2012/11/07/building-a-bipolar-supply-from-a-boost-converter/>

![](img/f350380cc1de65bcce032c24ab3710df.png "bipolar-supply-using-a-boost-converter")

[这款 DC-DC 双极 PSU](http://obsoletetechnology.wordpress.com/projects/studio-electronics/dc-dc-bipolar-power-supply-for-effect-pedals/) 是为配合吉他效果器踏板使用而开发的。[过时的技术]需要正负 15V 电源。如果你从市电转换，这是很容易做到的，但他想要一个能与低压交流/DC 壁式电源甚至电池一起工作的解决方案。

将这一切结合在一起的是 LT3467。这是一款开关电源调节器，通过少量外部无源器件的布局，提供一系列配置特性。它可以在每条线路(正极和负极)上输出 80 毫安。对于这种应用来说，芯片的高频操作也非常有用。根据不同的版本，它以 1.3 或 2.1 MHz 切换。这已经足够高了，不会在音响系统中引入可听见的噪音。

我们有一辆健身车，它的液晶负电源坏了。我们将尝试构建这个电路，根据我们的电压需求进行调整，并让对比度再次工作。

[谢谢奥利]