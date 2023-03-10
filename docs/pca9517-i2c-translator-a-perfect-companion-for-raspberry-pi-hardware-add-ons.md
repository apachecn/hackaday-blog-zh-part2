# PCA9517 I2c 转换器是 Raspberry Pi 硬件附件的完美伴侣

> 原文：<https://hackaday.com/2012/10/26/pca9517-i2c-translator-a-perfect-companion-for-raspberry-pi-hardware-add-ons/>

![](img/aa2f389a6673ef9d5afcd6290efdc552.png "wireless-temperature-sensing-with-rpi")

上图所示的装置是一个联网的温度传感器，它给[杰奥]发送一封电子邮件，显示随时间变化的图表。这本身很有趣，但有一部分特别吸引了我们的眼球。他使用 i2c 温度传感器，我们认为[PCA 9517 电平转换 I2C 总线中继器使](http://www.digitalexperience.eu/site/hw/r-berry-bash-2)成为 RPi 的完美匹配。

这是德州仪器的零件。你可以从该公司的产品页面找到更多相关信息。芯片名称中的关键词是“电平转换”。这有两个总线连接，每个都有可变的电压电平。在 A 侧，总线可以是 0.9V 至 5.5V。在 B 侧，总线范围是 2.7V 至 5.5V。由于 Raspberry Pi I/O 引脚以 3.3V 工作，因此可以连接到 B 侧，使您能够与额定电压较低或较高的 i2c 器件接口。这对于那些从 Arduino 开始并拥有大多数 5V 兼容原型硬件的人来说尤其方便。

该器件采用 SOIC 封装，你可以很容易地手工焊接，成本约为 1 美元，取决于供应商。