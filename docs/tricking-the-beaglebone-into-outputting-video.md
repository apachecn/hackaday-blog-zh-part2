# 欺骗小猎犬输出视频

> 原文：<https://hackaday.com/2012/06/26/tricking-the-beaglebone-into-outputting-video/>

![](img/aef8723216640aea2989067ba1d82260.png "beaglebone-video-output-trick")

[FlorianH]想让视频和他的小猎犬骨一起工作，但是他不知道如何让内核打球。然后，我突然有了一点灵感。他知道，如果你插入官方的 DVI cape(这是 BeagleBone 的单词，表示你可能知道的盾)，内核会自动开始发出他需要的信号。于是他想出了一个[的办法，恶搞海角，输出视频](https://sites.google.com/site/fpgaandco/fooling-the-beagle)。

在启动时，内核轮询 I2C 总线，看看连接了什么。DVI cape 有一个可识别它的 EEPROM。由于 EEPROM 中的数据可供下载，FlorianH 获取了他需要的数据，然后用 ATmega32 代替存储芯片。当他让芯片与喙骨对话时，他能够在他的瞄准镜上检测到视频同步信号，他知道他成功了。

仔细观察右侧的试验板。我们喜欢 ATmega32 银分线板。非常原型友好！