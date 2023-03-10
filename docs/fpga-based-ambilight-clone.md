# 基于 FPGA 的流光溢彩克隆

> 原文：<https://hackaday.com/2015/04/25/fpga-based-ambilight-clone/>

飞利浦流光溢彩——一束贴在电视背面的后置 RGB LEDs 正在成为任何开始摆弄 FPGAs 的人的标准项目。[DrX]的[是我们见过的最好的一款](http://zerocharactersleft.blogspot.com/2015/04/diy-fpga-based-hdmi-ambient-lighting.html)，有一个单板可以读取和 HDMI 流，让 blinkey 灯熄灭，并将 HDMI 流输出到电视或显示器。

[DrX]在这个项目中使用了带两个 HDMI 连接器的 FPGA 开发板——Scarab minispartan 6+—和一串 WS2801 可单独寻址的 RGB LEDs。通过一点电平转换，驱动 led 变得很容易。但是解码 HDMI 呢？

这个项目的大部分都是借用了一个在 720p 视频流的一角显示 logo [的项目。硬件是相同的，但是对于流光溢彩的克隆，你需要*读取*视频流并处理它，而不仅仅是写入它。通过仔细跟踪每个像素的 R、G 和 B 值以及像素时钟，可以对显示器边缘的颜色进行平均。它不像构建帧缓冲区那样困难，也不像构建帧缓冲区那样占用大量内存；当围绕显示器的周边集合平均值时，几乎所有的图像数据都被丢弃。不过，它确实有用。](http://hamsterworks.co.nz/mediawiki/index.php/MiniSpartan6%2B_DVID_Logo)

在计算出显示器周边的平均颜色后，驱动 led 就成了一件简单的事情。将这些发光二极管贴在电视背面，就有了一个用 FPGA 制作的流光溢彩克隆产品。

[DrX]有一些他的项目的视频。你可以看看下面这些。

[https://www.youtube.com/embed/SHEtCRncd2c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SHEtCRncd2c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/3aYjZszkyi8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3aYjZszkyi8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)