# [Sprite_tm]将一个 LCD 连接到一个微型 Linux 主板上

> 原文：<https://hackaday.com/2012/06/25/sprite_tm-connects-an-lcd-to-a-tiny-linux-board/>

![](img/4b1adb54603d56f79476584a885f6001.png "sprite")

[Sprite_tm]的一位同事最近向他挑战，让他将一个小型液晶触摸屏连接到一个树莓派上。可悲的是，[Sprite_tm]还没有交付树莓 Pi，但他确实设法将 LCD 连接到没有视频功能的 Linux 板上。

因为[Sprite_tm]的显示器有一个 16 位并行接口，并且 16 个 GPIO 引脚很难在[杨桃](http://www.8devices.com/product/3/carambola) Linux 板上获得，所以必须在构建中引入一些移位寄存器来使 LCD 工作。这些移位寄存器通过 SPI 接口连接到杨桃板；将所有 LCD 引脚连接到 Linux 板的一种非常简单的方法。

当然，如果没有内核驱动程序，Linux 就无法与 LCD 对话；[Sprite_tm]编写了一个 framebuffer 驱动程序，因此 LCD 可以用作控制台、X 会话，或者由任何其他可以写入 framebuffer 设备的程序使用。

像所有优秀的驱动程序作者一样，[Sprite_tm]正在分发补丁，以启用杨桃上的 SPI 化 LCD 面板以及移位寄存器原理图。幸运的话，当[Sprite_tm]收到他的树莓派时，我们还会看到 Raspi 驱动程序。