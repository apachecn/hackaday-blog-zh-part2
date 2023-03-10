# 3D 频谱分析仪使用 1280 个发光二极管

> 原文：<https://hackaday.com/2015/03/23/3d-spectrum-analyzer-uses-1280-leds/>

[Dooievriend]的一个朋友最近要求他为他制作的 3d 频谱分析仪/VU 编写软件。VU 是一个相当复杂的建筑:它由 16x16x5 矩阵中的 1280 个 led 组成，由 80MHz 时钟的 PIC32 控制。[Dooievriend]为 PIC 写了一些固件，这些固件使用离散傅立叶变换的变体来创建 3D VU 效果。

当[Dooievriend]着手设计固件的音频分析部分时，他想到了离散傅立叶变换。这种变换计算音频中一系列频段的振幅，看起来非常适合 VU。然而，在更多的研究之后，[Dooievriend]决定实现一个[常数 Q 变换](http://wwwmath.uni-muenster.de/logik/Personen/blankertz/constQ/constQ.html)。这种变换与傅立叶变换非常相似，但它考虑了人耳理解声音的对数方式。

[Dooievriend]开始使用基于中断的采样器实现常数 Q 变换，但他很快就遇到了他的 PIC32(没有硬件浮点单元)上的慢速浮点数学问题。谢天谢地，他用定点数学重写了代码，转换几乎是实时进行的。休息之后，请查看视频，了解 VU 的运行情况，第二个视频提供了硬件构建的一些细节。

[https://www.youtube.com/embed/yYPCe372meM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yYPCe372meM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Vn39txtVIHc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Vn39txtVIHc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)