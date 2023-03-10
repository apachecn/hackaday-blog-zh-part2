# 没有编程器的 AVR 编程器

> 原文：<https://hackaday.com/2012/09/14/avr-programmer-made-without-a-programmer/>

![](img/7c1771c58467dd52f58bf98a3bdc8028.png "avr-programmer-using-dfu")

【blueHash】用这个[廉价开发板做 AVR 编程器](http://atinkerslog.blogspot.com/2012/09/re-purposing-atmega32u4-as-avrisp-part-1.html)。我们感兴趣的是，它解决了在引导程序员时通常会遇到的先有鸡还是先有蛋的问题。我们[以前写过这个问题](http://hackaday.com/2010/10/25/avr-programming-02-the-hardware/)。大多数程序员使用微控制器，微控制器首先需要使用编程器进行闪存。但结果是[这个开发板上的芯片有一个 DFU 模式](http://atinkerslog.blogspot.com/2012/07/how-not-to-start-programming-with-avrs.html)，绕过了这个难题。

他以大约 6 美元的价格买了一个美元开发板。它有一个晶体，一个 ATmega32u4 芯片，另一边有一个 MicroSD 卡插槽。我们环顾四周，发现了一个描述设备固件升级机制的 [Atmel 数据表](http://www.atmel.cimg/doc7618.pdf) (PDF)。支持 DFU 的 AVR 设备在出厂时已配置为使用它。这个开发板是为使用 DFU 而设计的，所以[blueHash]需要做的就是找到并配置一个与这个芯片一起工作的 ISP 固件包。