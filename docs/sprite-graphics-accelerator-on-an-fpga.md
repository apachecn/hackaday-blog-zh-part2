# FPGA 上的 Sprite 图形加速器

> 原文：<https://hackaday.com/2014/08/15/sprite-graphics-accelerator-on-an-fpga/>

[![A demo running on a FPGA sprite accelerator](img/99718cb2628c4a30a247856b39503c88.png)](http://hackaday.com/2014/08/15/sprite-graphics-accelerator-on-an-fpga/sprite_accel/)

图形加速器将操作转移到硬件上，这样可以更快地执行。这是什么让你的树莓派体面地显示高清视频。[安迪]的最新产品是 2D 雪碧引擎，在 FPGA 上有硬件[加速图形。](http://andybrown.me.uk/wk/2014/06/01/ase/)

在最简单的模式下，sprite 引擎只是将命令传递给 LCD。这允许基本的控制。有趣的部分精灵模式，允许精灵加载到 FPGA 上。此时，您可以显示、隐藏和移动精灵。通过叠加许多精灵，你会得到类似上面演示的效果。

FPGA 来自 Xilinx，使用其块 RAM IP 来存储精灵的状态。实际的精灵数据包含在 128 Mb 的外部闪存芯片上，因为它们需要大量的空间。

游戏逻辑在 STM32 Cortex M4 微控制器上运行，该微控制器与 FPGA 通信并命令小精灵。然后，FPGA 处理生成帧并将其发送到 LCD 屏幕，从而释放微控制器。

如果你想知道 LCD 本身，它是 3.2 英寸，640 x 360，取自爱立信 U5 Vivaz 手机。[Andy]有一篇关于逆向工程 it 的详细[文章。休息之后，他给我们看了整个系统的视频。](http://andybrown.me.uk/wk/2013/10/19/vivaz-u5-lcd/)

[https://www.youtube.com/embed/UEIDRQzh_d0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UEIDRQzh_d0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)