# Stellaris Launchpad 库用于驱动 TM1638 UI 板

> 原文：<https://hackaday.com/2012/10/12/stellaris-launchpad-library-to-drive-the-tm1638-ui-board/>

![](img/b4f5f9ea0fda2b510f8c1cf0958df5c4.png "tm1638_stellaris_launchpad_library")

对于那些获得这些 TM1638 UI 板之一的用户，您现在可以通过 Stellaris Launchpad 轻松使用它。[Dan O]主动为 UI 板发布了[ARM 库。](http://trandi.wordpress.com/2012/10/11/tm1638-display-driver-for-stellaris-launchpad/)

这里没什么新东西可谈。我们已经看到这个[由 FPGA](http://hackaday.com/2012/09/19/using-an-undocumented-display-with-an-fpga/) 驱动。[Dan]还链接到主板的 Arduino 和 MSP430 库。值得一提的是，该板在 Stellaris Launchpad 提供的 3.3V 电压下运行良好。

ARM 芯片有四个不同的硬件 SPI 模块，可用于驱动该显示器。但是[丹]选择了咬刘海。这给了他更多的灵活性，像容易地改变引脚映射和放弃对外部元件的需要。只需直接连接用于时钟、数据输入和数据输出的三个 I/O 引脚。休息之后我们嵌入了强制性的演示视频。

[https://www.youtube.com/embed/pxv--nHNUzw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pxv--nHNUzw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)