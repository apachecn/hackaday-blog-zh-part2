# 用于 ECG、EEG 和其他测量的开放式硬件平台

> 原文：<https://hackaday.com/2014/08/13/an-open-hardware-platform-for-ecg-eeg-and-other-measurements/>

[Eric]向我们介绍了 OpenHarwareExG 项目，该项目的目标是构建一种允许创建电生理信号处理应用的设备。后者指的是[心电图](http://en.wikipedia.org/wiki/Electrocardiography) (ECG，心脏的活动)[脑电图](http://en.wikipedia.org/wiki/Electroencephalography) (EEG，头皮上的信号)[肌电图](http://en.wikipedia.org/wiki/Electromyography) (EMG，骨骼肌活动)[眼震电](http://en.wikipedia.org/wiki/Electronystagmography)和[眼电](http://en.wikipedia.org/wiki/Electrooculography) (ENG & EOG，眼球运动)监测项目。正如你所猜测的，这些信号由于幅度小，对电噪声非常敏感，因此特别难以测量。

该平台中使用的 ADS1299 8 通道 24 位模拟前端实际上与电路的其余部分电气隔离，因此 USB 连接不会干扰测量。使用 Arduino 兼容的 ATSAM3X 微控制器，所有电路板都是“DIY 兼容”的，因为所有器件都可以少量采购并手工焊接。甚至连外壳都是开源的，由丙烯酸树脂激光切割而成。

前往该项目的网站下载所有的源文件，并观看该系统运行的快速视频。

对测量身体的潜能感兴趣？检查一个足以让你知道你已经死亡的[心电图](http://hackaday.com/2014/02/13/arduino-powered-ecg-informs-users-of-their-death/)，或者这个[基于 Android 的无线](http://hackaday.com/2014/06/05/android-based-wireless-ecg/)设置。