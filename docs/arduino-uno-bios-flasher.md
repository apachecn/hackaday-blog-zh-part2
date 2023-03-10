# Arduino Uno BIOS 闪屏

> 原文：<https://hackaday.com/2012/05/04/arduino-uno-bios-flasher/>

![](img/9ad1b111e3c6a344449729fd71f4a03e.png "arduino-uno-bios-flashing")

我们已经见过几次 Arduino 用来刷新 BIOS 芯片。但这些黑客攻击几乎总是由糟糕的闪存造成的。这一次[GNUtoo]感兴趣的是将一个工具放在您的手中，它可以用来将 Coreboot 闪存到您的主板上。他的产品使用 Arduino Uno ，但也包括其他几个硬件选项。

固件利用写入闪存芯片时制作的 serprog-duino 库。在电脑方面[flash rom 包](http://www.flashrom.org/Flashrom)将 BIOS 镜像推送到 Arduino。好的一面是 flashrom 是 Linux 仓库中的一个常见包，所以它可能只是一个简单的方法。

这一过程并不算快，对一个 1 Mb 的芯片编程只需 10 分钟左右。但是如果你只是对[加载开源 BIOS 替代品](http://www.coreboot.org/Welcome_to_coreboot)感兴趣，这很容易设置。