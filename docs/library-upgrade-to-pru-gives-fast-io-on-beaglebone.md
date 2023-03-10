# 库升级到 PRU 在 Beaglebone 上提供快速 IO

> 原文：<https://hackaday.com/2015/02/16/library-upgrade-to-pru-gives-fast-io-on-beaglebone/>

BeagleBone Black 有一个强大的功能集:像样的时钟速度，模拟输入，多个 UART，SPI 和 I2C 通道和板载存储器，等等。一个缺失的特性似乎是缺少对两个板载可编程实时单元(PRU)的支持。每个 32 位处理器都独立于主处理器运行，但能够通过使用共享 RAM 和一些中断与主处理器接口。不幸的是，PRU 不被支持，并且在缺乏信息的情况下，难以编程。例如，启用 PRU 将允许它们通过 GPIO 引脚直接访问外部传感器。或许最吸引人的想法是保诚为 BBB 增加实时处理能力。

[Thomas Freiherr]正在进行[libpruo](http://beagleboard.org/project/libpruio/)项目，以允许保诚支持 BBB。它“旨在方便配置和高速数据处理。libpruio 软件在主机(ARM)上运行，同时在可编程实时单元子系统(= PRUSS 或只是 PRU)上运行，并控制这些子系统”。关于这个项目的更多信息可以在 libpruio wiki 上[获得，文件可以从这里](http://users.freebasic-portal.de/tjf/Projekte/libpruio/doc/html/)(德语页面)[下载。](http://www.freebasic-portal.de/downloads/fb-on-arm/anleitung-zu-libpruio-en-326.html)

几个月前在 inter.noise2014 (PDF)上发表的这篇[论文对各种小型计算机/控制器板进行了很好的比较，并概述了启用 pru 后 BBB 的优势。如果读者遇到启用 PRUs 的 BBB 应用程序，请在评论中告诉我们。如果你想进入保诚](http://www.acoustics.asn.au/conference_proceedings/INTERNOISE2014/papers/p236.pdf)[的世界，我们强烈推荐这个系列教程](http://hackaday.com/2014/06/22/an-introduction-to-the-beaglebone-pru/)。

[Patrick]感谢您发送提示

【图片来源: [libpruio 步进电机示例](http://users.freebasic-portal.de/tjf/Projekte/libpruio/doc/html/_cha_examples.html#SubSecExaStepper)