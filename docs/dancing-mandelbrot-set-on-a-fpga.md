# 在 FPGA 上设置跳舞的 Mandelbrot

> 原文：<https://hackaday.com/2015/05/26/dancing-mandelbrot-set-on-a-fpga/>

这种基于 FPGA 的构建创建了一个有趣的显示，对音乐做出反应。【万成】[跳舞的曼德尔布罗集](https://hackaday.io/project/5860-let-mandelbrot-set-dance-with-music)使用 FPGA 和一些数学来生成可控的分形显示。

构建产生一个 [Mandelbrot 集合](http://en.wikipedia.org/wiki/Mandelbrot_set),其颜色由音频输入修改。承载 Cyclone IV FPGA 的 Terasic DE2-115 开发板提供所有 IO 和处理。在输入端，UART 或 IR 遥控器可用于放大和缩小显示屏。音频输入映射到颜色控制，VGA 输出允许实时显示结果。

在 FPGA 上，一个运行频率高达 150 MHz 的自定义计算引擎执行数学运算，生成分形。快速傅立叶变换将音频输入分解成频率，这些频率用于控制输出图像的颜色。

这种构建最好通过观看来解释，所以休息后查看视频。

[https://www.youtube.com/embed/epDKXIOjEI4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/epDKXIOjEI4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)