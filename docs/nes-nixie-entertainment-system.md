# NES:谢妮娱乐系统

> 原文：<https://hackaday.com/2013/09/11/nes-nixie-entertainment-system/>

![nixieNES](img/7cc70d50e013019331b03406ad63aa23.png)

[Bradley W. Lewis]对谢妮时钟制造并不陌生，他觉得他最近的委托缺少了一些东西。他不再仅仅将谢妮钟安装在一个类似 NES 控制台的盒子里，而是全力以赴，将它变成了一个 NES 控制台模拟器。在铣床上做了一些工作后，一个木箱就有了空间，可以塞进一些新部件。[Bradley]最初计划只安装一个带有 ArduNIX 屏蔽的 Arduino 来处理谢妮时钟，但是仿真器要求节省一些空间。翻转 Arduino 的一侧可以腾出足够的空间，屏蔽仍然可以轻松地连接到相邻的 Nixie 管板。

Raspberry Pi 用作控制台仿真器，安装在靠近机箱的一侧，以便访问其 HDMI 端口。Arduino 和 RasPi 的其他端口都从后面伸出来，包括 Pi 的 RCA 视频输出的扩展和设置时钟小时和分钟的按钮。表壳前面的两个多余的 NES 按钮控制 RasPi 的电源，并为谢妮时钟提供复位功能。

如果谢妮还不够让你满意，那就去看看无线谢妮柜台。