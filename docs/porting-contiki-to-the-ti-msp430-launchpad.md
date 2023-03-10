# 将 Contiki 移植到 TI MSP430 启动平台

> 原文：<https://hackaday.com/2014/01/07/porting-contiki-to-the-ti-msp430-launchpad/>

[![](img/50098835d62676e183cb60c01d313004.png)](http://hackaday.com/wp-content/uploads/2014/01/lpcc2500picoscope.jpg)

多年来，在选择 IPv6 而不是低功耗无线个人区域网堆栈(又名 [6LoWPAN](http://en.wikipedia.org/wiki/6LoWPAN) )时，Contiki 一直是主要选择之一。它是由一个世界范围的开发团队开发的，Atmel、Cisco、ETH 等都有贡献，而是开源的。由于大多数移植了 Contiki 的平台都非常昂贵，【Marcus】决定[将操作系统带到 TI Launchpad](http://www.bithappens.se/blog/2013/05/26/contiki-for-ti-msp430-launchpad/) 。对于不知道的读者，后者基于 msp430g2452/2553 微控制器，只有 256/512 字节的 RAM 和 16kB 的 ROM。顺便说一下，Contiki 通常需要 10k RAM 和 30k ROM。

[Marcus]因此不得不删除 Contiki 的几个功能:队列缓冲、能量估计和令人遗憾的 uIP。他的测试设置(如上所示)使用 TI CC2500 无线电，在 Aliexpress 上可以以不到 2 美元的价格找到，他为此从头开始编写无线电驱动程序。他还编写了自己的无线电循环层，因为 Contiki 中包含的那个太大了。