# 你的菜园浇水系统

> 原文：<https://hackaday.com/2012/08/15/watering-system-for-your-vegetable-garden/>

![](img/77f54a14b80c92c1a356ac4650ab4255.png "auto-watering-system")

多亏了 Dillon Nichols 建造的自动浇水控制器，当他度假回来时，这些蔬菜还会活着。这是该项目的第二次迭代，主要处理更换控制器本身的电子设备和 UI。他[在之前的帖子中详细介绍了用于浇灌](http://tinkeringetc.blogspot.com/2012/06/automatic-garden-waterer-part-1.html)的硬件。他在一个电磁阀上接上了水管，水管的输出端穿过花园的花坛。这是一个常开阀，但我们建议使用常闭阀，因为停电会让软管持续运行。

[Dillon]在 Arduino 板上进行原型设计，然后转移到某个原型板上的独立 ATmega328 芯片上进行最终设计。他使用 3D 打印机制作了定制面板，允许访问三个控制按钮，并为字符 LCD 提供了安装位置。除了定时器设置，还有一个手动浇水开关。他使用了一个典型的电源灯开关，用下拉电阻连接，使其与 Arduino 配合良好。他对计时器系统的解释可以在休息后看到。

[https://www.youtube.com/embed/riKKSQhLVXc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/riKKSQhLVXc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)