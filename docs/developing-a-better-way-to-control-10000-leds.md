# 开发更好的方法来控制 10，000 个 led

> 原文：<https://hackaday.com/2012/07/31/developing-a-better-way-to-control-10000-leds/>

![](img/3936dddddd010eea564c5a9a996fa0f1.png "10000-led-control")

SoundPuddle 项目基于音频输入驱动数千个 led。该团队正在用更强大的东西来替换这个电线填充设置的控制器。他们把上面看到的混乱带到[的 Apogaea 节](http://apogaea.com/the-apogaea-festival/)，由于噪音和干扰，他们被松散的电线和不可靠的通信所困扰。新系统的目标是可靠地控制多达 10，000 个 led。

在鼠窝中央看到的红色 PCB 是一个凤蝶 FPGA 板。他们仍然想用它来驱动安装，但是需要一个新的硬件接口。解决办法是设计他们所谓的巨型翅膀(翅膀对于凤蝶就像盾牌对于 Arduino 一样)。led 将采用 RGB 条形，因此要求之一是提供足够的连接器来驱动 16 通道 SPI 器件。机翼还将包括 48V 电源和电容麦克风的连接器，电容麦克风用作声音池的输入。音频输入还有两种选择，一种是通过蓝牙模块(可以兼作控制设备)，另一种是通过 MIDI。

休息之后，你可以看到一个灯光演示。准备好音量控制，因为测试中使用的大多数声音都很烦人。

[https://www.youtube.com/embed/wX3d7aHBEWY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wX3d7aHBEWY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢查理]