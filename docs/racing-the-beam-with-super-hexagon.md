# 用超级六边形比赛平衡木

> 原文：<https://hackaday.com/2015/05/13/racing-the-beam-with-super-hexagon/>

像 Atari 2600 这样的早期游戏机的内存非常非常有限。甚至没有足够的内存来容纳屏幕上的所有像素；相反，像素是在绘制时由 CPU 生成的。它用代码玩扫描线和彩色半身像，我们现在称之为。因为某种原因在比赛平衡木。

[Sam]正在攻读电子工程学位，为了一门数字设计课，他需要编写一些 Verilog。当时他沉迷于超级六边形游戏，游戏机制对于 FPGA 来说非常简单。他构建了自己的实现，但不是带帧缓冲区的。他使用流水线方法，在显示之前的几个时钟周期内计算每个像素的值。与 framebuffer 方法相比，它大大降低了 Altera DE1 板上的内存需求。

下面视频。

[https://www.youtube.com/embed/GWpCRnAXXIU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GWpCRnAXXIU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)