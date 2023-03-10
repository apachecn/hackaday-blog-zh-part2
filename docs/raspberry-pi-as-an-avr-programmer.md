# 作为 AVR 程序员的 Raspberry Pi

> 原文：<https://hackaday.com/2012/08/20/raspberry-pi-as-an-avr-programmer/>

![](img/b6b367ccd92c36d168543b58ad4cd7d4.png "avr")

AVR 程序员可以在网上花几美元买到，但如果你正在为你的 Raspi 构建一个带有 AVR 的扩展板，[这就是为你构建的](http://blog.stevemarple.co.uk/2012/07/avrarduino-isp-programmer-using.html)。通过 Raspi 的 GPIO 引脚对 AVR 进行编程是一种安全的方式，使用的电路极其简单。

AVR ISP 接口看起来很像 SPI 接口，用 Raspi 对 AVR 编程的最简单方法是从 GPIO 引脚 bitbang 所有命令。不过，有时 AVR 和 Raspi 的逻辑会在不同的层次上，所以虽然 bitbanging 可能在紧要关头工作，但它不是任何人都应该经常使用的东西。

为了让 Raspi 和 AVR 安全地相互通话，[Steve]用一个 74244 缓冲器和一个 FET 构建了一个小电路。由于增加了对 Linux GPIO avrdude 编程的支持，用 Raspi 编程 AVR 变得轻而易举。

几天前，我们遇到了一个过度紧张的 PIC 程序员，所以我们很高兴看到 PIC/AVR 圣战的另一轮转向 AVR 阵营。

感谢[Mateusz]发送此邮件。