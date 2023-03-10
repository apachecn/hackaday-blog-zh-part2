# 把所有东西都塞进 DIP32 封装

> 原文：<https://hackaday.com/2015/08/30/stuffing-everything-on-a-dip32-package/>

将一个完整的微控制器平台放入 DIP 格式并不是什么新鲜事 Teensy 做到了，Arduino nano 做到了，其他十几个电路板也做到了。[Alex]和[Alexey]不满足于仅仅一个简单的微控制器分线板，所以他们在基本的 Arduino 平台上添加了一个无线电、一个有机发光二极管、一个 SD 读卡器，甚至更多的 RAM，[所有这些都在一个小的、易于使用的封装中](https://hackaday.io/project/7436)。

[Alex]和[Alexy]称之为 DIPDuino，它具有 ATmega1284 处理器。为此，他们增加了一个 128×32 像素的有机发光二极管，一个微型 SD 插槽和 1mb 的 SRAM。微控制器[是一个变体](http://www.atmel.com/devices/ATMEGA1284RFR2.aspx)，它包括一个 2.4 GHz Zigbee 无线电，允许无线连接到其他显示器。

(亚历克斯)和(阿列克谢)打算用他们那块很酷的小木板做什么？他们计划将有机发光二极管用于手表，改进他们的软件，以便可以从 SD 卡更新固件，而[Alex]的一个朋友想用其中的一个来制作 RepRap 控制器。这块板有很大的潜力，我们很想看看这些人会把这个项目带向何方。