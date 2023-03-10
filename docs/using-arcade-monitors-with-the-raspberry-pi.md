# 将街机显示器与 Raspberry Pi 配合使用

> 原文：<https://hackaday.com/2012/12/17/using-arcade-monitors-with-the-raspberry-pi/>

![mame](img/ed58f10fd36297443be7385fad503b22.png)

随着树莓派越来越受欢迎，我们也看到了 MAME 拱廊橱柜的相关上升。将这台 35 美元的电脑放在街机机柜中很有意义，但将它连接到旧街机机柜中的显示器上有点痛苦。幸运的是，[Celso]想出了如何将一个 Raspi 连接到这些 15kHz RGB 显示器中的一个，从而更准确地模拟旧的街机经典。

Raspi 只有两个视频输出-一个 HDMI 端口和一个 RCA 复合插孔。旧的 arcade CRTs 有一个 RGB 输入，因此直接将 Raspi 连接到这些 CRT 是不可行的。

该解决方案来自两个转换器:一个将 HDMI 输出转换为 VGA，另一个视频降频器接收 31kHz VGA 信号，并将其转换为 15kHz RGB 信号。[塞尔索]选定了 [GBS-8100 视频转换器](http://www.digitalsystemsdesign.co.uk/product_uploads/13153855771.pdf)，这是一个相当罕见的套件，幸运的是在一些中国易贝拍卖会上可以找到。

在将旧的街机机柜电源连接到 Pi，连接上音频放大器，并将控制转换为 USB 之后，[Celso]拥有了一台非常精确的 MAME 机器。