# 三星 S-Pen 的逆向工程

> 原文：<https://hackaday.com/2015/02/22/towards-a-reverse-engineering-of-samsungs-s-pen/>

几年前，所有这些酷图形平板电脑背后的公司 Wacom 与三星合作，创造了 S Pen，这是上世纪 90 年代发生的怪异笔式计算的重生，也是一种非常有趣的外设，只要有人能为它编写一些软件。[Kerry D. Wong]想知道 S Pen 是如何工作的，于是[连接了一些硬件，看看 S Pen 是如何与手机](http://www.kerrywong.com/2015/02/15/samsung-galaxy-s-pen-waveform-capture/)通信的。

众所周知，S Pen 是由射频场驱动的，工作原理有点像 RFID。监听通讯需要某种线圈，所以[凯瑞]拆卸了一个小扬声器，并将其连接到一个示波器上。

从 S Pen 捕获的波形来看，载波频率似乎在 550 到 560kHz 的范围内，超出了标准 RFID 的范围。他没有解码完整协议的设备，但可以推断出一些事情——屏幕通过检测射频场强的下降来感应笔的位置。笔和电话之间传输的唯一信息是 11 位压力敏感度和一个 1 位值，该值表示按钮是开还是关。

[Kerry]把波形数据放到他的网站上，如果有人想尝试解码协议。