# 我们是博格人。我们会给你的视觉增加热量和距离感。

> 原文：<https://hackaday.com/2012/12/20/we-are-the-borg-we-will-add-heat-and-distance-sensing-to-your-vision/>

![we-are-borg](img/c3b0c5b631f4b90b5ba6ab0564116631.png)

[Gregory McRoberts]出生时一只眼睛视力下降，从未体验过我们大多数人认为理所当然的三维视觉。最近，他受到助听器概念的启发，制造了一种可以增强视力的设备。看，他戴着的非常像博格人的眼罩为他的感官调色板增加了距离和热量。

他选择的硬件是兼容 Arduino 的 Lilypad 板。它被连接到一个超声波测距仪和一个红外线传感器上，用来监控他前方的区域。他右眼的功能仍然能够看到光和颜色，因此在内部安装了一对 LED 板。一个连接到热传感器，当低于 80 华氏度时显示蓝色，当高于 80 华氏度时显示红色。另一个 LED 为绿色，根据距离传感器的读数以不同的速度闪烁。

由于发光二极管的强度，当视力正常的人戴上它时，会分散注意力。我们发现[格雷戈里]对此的解释(称为[头盔着火](http://en.wikipedia.org/wiki/Helmet_fire))相当有趣。

[途径 [Adafruit](http://www.adafruit.com/blog/2012/12/19/augmented-vision-eyepatch-wearablewednesday/)