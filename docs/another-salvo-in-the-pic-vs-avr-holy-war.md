# 另一个齐射的图片对 AVR 圣战

> 原文：<https://hackaday.com/2013/03/10/another-salvo-in-the-pic-vs-avr-holy-war/>

啊，PIC vs. AVR，永无止境的电子设计霸主之战。有些人对 Atmel 的 AVR 微控制器信誓旦旦，有些人却错了。[majenko]坚定地站在 Microchip 的 PIC 阵营，所以他[写了一份 Atmel 的 AVR 与 Microchip 的 PIC 系列微控制器](http://digital-diy.com/pic-micrcontroller/532-why-i-pick-pic.html)的很好的比较。结果并不令人惊讶；PIC 微控制器是一个没有爱好者使用的更好的产品，因为没有爱好者使用它们。

过去几年，Atmel 及其 AVR 微控制器系列在业余爱好者市场中的受欢迎程度大幅提高，这无疑要归功于 Arduino 和其他 AVR 驱动的开发板。这并不是说 Microchip 和 PIC 还没有看到他们的时代；曾经有一段时间，你可以在 Radio Shack 买到电子元件，包括含有微芯片非常受欢迎但有点过时的基本印章的套件。

在检查了 Atmel AVR ATMega328p、类似配置的 Microchip 的 PIC18F25K80 和 TI 的 MSP430G2533 的功能后，[majenko]发现多年来最受欢迎的 AVR 在一些非常重要的类别中缺乏。AVR 具有更低分辨率的 ADC、更少的 PWM 引脚、更少的 16 位定时器，而成本大约多 0.75 美元。

当然[majenko]的分析没有考虑到选择 PIC 而不是 AVR 的无形因素。由于 Arduino 采用了 AVR，几乎所有可以想象的项目都有更多的代码和示意图在互联网上流传。PIC 的开发工具比 AVR 的同类产品要贵一些；一个 PICkit2 大约需要 50 美元，而 AVR ISP 程序员几乎随处可见。

这是一个慵懒的星期天，所以你们可以在评论中继续争论。