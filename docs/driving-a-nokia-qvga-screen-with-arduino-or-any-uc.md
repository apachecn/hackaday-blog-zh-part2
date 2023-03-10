# 用 Arduino(或任何 UC)驱动诺基亚 QVGA 屏幕

> 原文：<https://hackaday.com/2012/06/20/driving-a-nokia-qvga-screen-with-arduino-or-any-uc/>

![](img/7ad375eb82ee1244697939f2e4c9af73.png "nokia-qvga-tft-from-arduino")

这是诺基亚 6300 的屏幕。这是一个 320×240 的显示器，具有大约 2 英寸的对角线观看区域，并拥有 24 位 QVGA TFT 技术。在你的下一个项目中，它会看起来很棒，并且由于[安迪·布朗]将硬件和[软件指南](http://andybrown.me.uk/wk/2012/06/04/nokia-qvga-tft-lcd-for-the-arduino-mega-graphics-library-part-2-of-2/)放在一起，它不会很难启动和运行。他选择这种显示器是因为它的特点，但也因为它真的很容易获得，并且只需 5-7 美元即可获得。该指南旨在使用 Arduino MEGA，但我们确信您可以将其移植到任何您喜欢的微控制器上。

与我们刚刚看到的 FPGA PSP 显示器非常相似，[Andy]选择设计自己的 PCB 来承载 LCD。这使得连接 LCD 变得轻而易举——实际上，因为他设法找到了正确的嵌入式连接器。该板还拥有一个恒流 LED 驱动器，负责背光，并允许他内置一个电平转换器(因为屏幕以 3.3V 通信，但 Arduino 使用 5V 逻辑)。

软件教程很长，但令人印象深刻。我们对他从 AVR 芯片中获得的性能感到惊讶。休息之后，观看屏幕循环播放一组演示。

[https://www.youtube.com/embed/CVV5ri9Cx_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CVV5ri9Cx_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)