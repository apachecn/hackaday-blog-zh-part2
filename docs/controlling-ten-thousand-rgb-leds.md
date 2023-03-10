# 控制一万个 RGB LEDs

> 原文：<https://hackaday.com/2014/01/02/controlling-ten-thousand-rgb-leds/>

RGB LED 棒极了——尤其是采用 WS2812 RGB LED 驱动器的新颖别致的 LED。这些 led 可以单独控制以显示红色、绿色和蓝色，但将它们与微控制器或计算机连接会带来一个问题:微控制器通常没有足够的 RAM 来存储图像，并且具有足够内存来做一些事情的设备没有实时操作系统，也没有能力做这些 led 需要的非常精确的定时。[Sprite_tm]思考了这个问题，并提出了一个控制所有 WS2812 LEDs 的伟大解决方案[。](http://spritesmods.com/?art=imx233-ws2811)

[Sprite]发现在当前的 ARM/Linux 主板上有一个设备可以提供驱动大量 WS2812 LEDs 所需的极其精确的时序:视频接口。即使这些板上的视频接口是数字的，也可以将 [oLinuXino Nano](https://www.olimex.com/Products/OLinuXino/iMX233/iMX233-OLinuXino-NANO/) 上的 16 位 LCD 接口转变为以一致的时序快速输出数字值的接口。这正是大量 RGB 像素所需要的。

使用 Linux 板通过视频输出驱动 RGB 像素意味着[Sprite_tm]需要视频输出。他运行的是最新的 Linux 内核，所以他没有驱动程序来启用视频硬件。这对[Sprite]来说不成问题，因为他只需添加几个文件来定义 16 位 LCD 界面并添加适当的显示模式。

[Sprite_tm]在模拟 16 条 600 个 led 时，已经将示波器带到他的板上，并且能够获得 30 fps 的帧速率。这相当于由一块 22 美元/30 美元的€电路板控制近 10，000 个 led。

现在，建造一个巨大的 LED 显示屏的唯一障碍实际上是购买 RGB LED 灯条。简单算一下，640×480 的显示屏光是 led 就要 50，000 美元。有人知道哪里可以买到便宜的 LED 灯吗？

[https://www.youtube.com/embed/WVbBAxcVX3k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WVbBAxcVX3k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)