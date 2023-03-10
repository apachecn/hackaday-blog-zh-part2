# 一个真正的树莓派克隆(不是“灵感来自”)

> 原文：<https://hackaday.com/2014/07/30/a-real-raspberry-pi-clone-not-inspired-by/>

![odroid](img/78dda567f8ab69962b605336e8ab4ffe.png)几年前，Broadcom 有一款非常好的芯片——BCM 2835——可以处理 1080 视频，具有相当强大的图形性能，运行速度很快，而且相当便宜。一位博通员工想，“我们为什么不用这个造一台教育电脑呢”，树莓派就这样诞生了。从那时起，Broadcom 就一直保留着这些芯片，将它们全部集中到一个非常活跃的平台上，用于教育、修补和任何其他可以使用小型 Linux 板的项目。最近，Broadcom 已经开始向任何有现金的人出售 BCM2835，从它的外观来看，[真正的树莓 Pi 克隆开始进入市场](http://www.hardkernel.com/main/products/prdt_info.php?g_code=G140610189490)。

其他树莓 Pi 克隆板，如[香蕉 Pi](http://www.bananapi.org/) 和[鹰嘴豆板](http://www.solid-run.com/products/hummingboard/linux-sbc-specifications/)不使用 Raspi 和新 Odroid 中的 BCM2835。新板也有相同的 26 针 GPIO 扩展插座，运行与 Raspberry P 相同的二进制文件；。从任何意义上来说，它都是一个克隆，具有稍微不同的外形，适合非常小、便携和电池供电的使用场合。

与官方的 [Raspberry Pi 计算模块](http://www.raspberrypi.org/raspberry-pi-compute-module-new-product/)不同，Odroid 并不意味着被用作模块上的系统，而是被塞入任何需要快速 ARM 内核的产品中，而不需要工程师实际*设计*带 ARM 的电路。Odroid 是 Raspi 的精简版，非常适合任何空间紧张的项目。

Odroid 上有几个有趣的功能:有一个板载电池连接器，板上有一个实时时钟，更多的 BCM2835 GPIOs 暴露在外(尽管与升级的 [RPi Model B+](http://hackaday.com/2014/07/14/the-raspberry-pi-model-b-is-here-again/) 不是同一款)。没有以太网，但如果你正在建造电池供电的东西，你也不需要它。

就价格而言，[你可以花 30 美元从这些 Odroids](http://www.hardkernel.com/main/products/prdt_info.php?g_code=G140610189490) 中挑选一个，韩国运费 9 美元。这与真正的 Raspberry Pi 的价格相当，但如果 Odroid 中的功能对您来说值得，它可能是一个值得的克隆。