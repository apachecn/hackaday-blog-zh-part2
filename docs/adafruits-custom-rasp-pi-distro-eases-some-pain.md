# Adafruit 的自定义 Rasp Pi 发行版减轻了一些痛苦

> 原文：<https://hackaday.com/2012/08/03/adafruits-custom-rasp-pi-distro-eases-some-pain/>

![](img/a2ba83c3743338688eba1a6fb67fd986.png "adafruit_pi")

你们中的许多人还没有收到你的树莓派。当你这样做时，你会发现在操作系统中有工作要做，以使事情按你希望的那样工作。Adafruit 的优秀员工已经解决了这个问题，他们发布了自己的覆盆子 Pi Linux 发行版。

基于发货的发行版“Wheezy ”, Adafruit 的发行版“Occidentalis v 0.1 . Occidentalis . Rubus Occidentalis”或“the Black Raspberry”现在包括以下内容:

*   [更新至 Hexxeh 固件](https://raw.github.com/Hexxeh/rpi-update/master/rpi-update)
*   4g 标清图像(不适合 2 G 卡！)
*   I2C 和硬件 SPI 支持
*   I2C/SPI 模块在启动时初始化
*   启动时的 sshd
*   第一次启动时的 ssh 密钥生成
*   运行 ahavi 守护进程(Bonjour 客户端)并被称为 **raspberrypi.local**

*   [加载时 GPIO #4 上的一个电线支架](https://github.com/FrankBuss/linux-1/commit/71871509238d3e7bce4a74cdf616c3f12542acaa)