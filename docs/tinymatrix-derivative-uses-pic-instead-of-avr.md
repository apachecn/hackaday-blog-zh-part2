# TinyMatrix Derivative 使用 PIC 代替 AVR

> 原文：<https://hackaday.com/2012/10/22/tinymatrix-derivative-uses-pic-instead-of-avr/>

![](img/49eb60f95ae3c1844d9856207803828d.png "tinymatrix-using-pic")

[斯图]有一个十几岁的侄女的生日快到了，他想给她一个独特的礼物。他正在研发一款 LED 矩阵挂件，可以显示像素图形、播放动画和滚动信息。

在从 TinyMatrix 项目中获得灵感后，他开始了这项工作。这个巧妙的设计使用了直接焊接到 5×7 LED 矩阵引脚上的 DIP AVR 芯片。它由一个硬币电池供电，电源线和地线充当吊坠的项链。[Stu]更喜欢使用 PIC 芯片进行开发，所以他的项目基于 16F88。它不能在 3V 电源下运行，所以在最终设计完成之前，他有一些问题要解决。

很有趣的一件事是他的副业。在厌倦了为动画的每一帧手工编码数组之后，他用 C#编写了一个 GUI，让他可以设计图像并通过点击几下鼠标输出代码。