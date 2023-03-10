# 不使用 ADC 的 Raspi ADC

> 原文：<https://hackaday.com/2014/07/13/adc-for-raspi-without-using-an-adc/>

![Schematic of ACD for a raspi](img/12419540b87898f880bafea7b1eaa8d8.png)

树莓 Pi 可以做所有令人惊讶和美妙的事情，但它非常缺乏专用的 ADC 芯片。当然，您可以通过 SPI 甚至 I2C 来连接 ADC，但仍然需要做一些工作。如果能有一个模数转换器就好了，而不必麻烦。幸运的是，[胡萨姆]已经找到了一种方法来做到这一点。

使用一个比较器、两个电阻、一个电容和几行代码，[Hussam]成功地让一个有源 ADC 在他的 Raspberry Pi 上工作。他使用 PWM1 和一个无源 RC 滤波器来制作 DAC。然后，他使用比较器和“逐次逼近算法”来完成 ADC。

[Hussam]提到黑客攻击并不新鲜，这种技术以前曾用于缺乏内置 ADC 的微控制器。但我们仍然对他在描述如何在 Raspi 上做这件事时对细节的关注印象深刻。请务必查看完整的细节、代码和关于他的算法如何工作的精彩描述的链接。