# TI Launchpad 作为 AVR ISP 程序员

> 原文：<https://hackaday.com/2012/05/03/ti-launchpad-as-avr-isp-programmer/>

![](img/99bf8f0bdeff3eaec9046fc40fed762d.png "lauchpad-avr-isp-programmer")

[Minifloat]正在使用他的 [TI Launchpad 开发板作为 AVR 芯片](http://www.mikrocontroller.net/articles/Launchprog) ( [翻译](http://translate.google.com/translate?hl=en&sl=auto&tl=en&u=http%3A%2F%2Fwww.mikrocontroller.net%2Farticles%2FLaunchprog))的系统内程序员。有很多自制 AVR 程序员，在 ISP 上使用 Arduino 非常流行。但最近我们搜索了一种作为程序员使用 Launchpad 的方法，没有找到。我们敢说这是第一次。

必须对硬件进行一项修改。电路板上必须安装一个外部时钟晶体(32.768 kHz)。但是因为它是为这个特性而设计的，所以这是一个相当快的过程。[Minifloat]遵循了 Atmel 的 ISP 应用程序说明，并扩展了为不同的程序员编写的一些代码，以使事情正常运行。起初，设备不会与 AVRdude 通信，但这证明是初始化对话的问题。AVRdude 轮询连接的编程器以查看它是否支持块模式，而 MSP430G2211 上的固件不期望此查询。问题已经解决，现在可以工作了。

听起来系统里还有几个漏洞。AVRdude 在插入 USB 端口后第一次访问编程器时会失败。后续尝试将会成功，直到 MSP430 芯片复位或 USB 连接被重新插入。但如果你刚刚进入 AVR 行业，这将让你明白你是否想投资一个合适的程序员。