# 基于新 Stellaris 发射台构建的频率分析仪

> 原文：<https://hackaday.com/2012/09/06/frequency-analyzer-built-from-the-new-stellaris-launchpad/>

![](img/b147fee9fd831df2236695c2d6079c7c.png "stellaris-launchpad-frequency-analyzer")

这是我们看到的新 Stellaris Launchpad 的第一个项目。这是一个在 8×8 LED 模块上显示图形的频率分析仪。你说什么？您还没有收到新的 Launchpad 板吗？我们也没有，因为[他们要到月底才开始发货。但[EuphonistiHack]是 TI 的软件开发人员，并获得了一个早期开发部门。](http://hackaday.com/2012/08/31/preorder-tis-arm-cortex-m4-launchpad-for-5-delivered/)

硬件相当简单。他使用运算放大器将音频从笔记本电脑传输到 ARM 处理器。8×8 LED 模块是一个 MSP430 升压包，通过 SPI 寻址。在软件方面，他真正利用硬件外围设备来简化工作。定时器触发每个 ADC 读数，ADC 利用 uDMA 写入数值。然后使用数字信号处理(许多 ARM 芯片都有 CMSIS 库)将 ADC 值转换为可以在 led 上显示的值。休息之后，请观看视频，以了解最终版本。

Hackaday 的作者们正在为这个硬件寻找一个比“Stellaris Launchpad”更容易的名字。它似乎不适合一个更短的名字，就像 RPi 或 Raspi 为 Raspberry Pi 取的名字一样。如果你为新的版块起了一个吸引人的昵称，请在评论中分享。