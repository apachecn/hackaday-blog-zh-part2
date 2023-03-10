# Arduino Zero 硬件不仅仅是为新手准备的

> 原文：<https://hackaday.com/2014/05/21/arduino-zero-hardware-is-not-just-for-beginners/>

我们在 Maker Faire 的 Atmel 展台前停下来，呆呆地看着他们展示的预生产 Arduino Zero 主板。[鲍勃]给了我们一份新主板提供的所有东西的概要，它比我们上周[听说它时想象的要好。](http://hackaday.com/2014/05/15/introducing-the-arduino-zero/)

我可能是个怪人，因为我不喜欢在开发 uC 固件时使用 IDE。一般来说，我会使用 8 位的文本编辑器和 makefile，在使用 ARM 时会添加 OpenOCD 和 GDB。对于 Arduino Zero 已经有 OpenOCD 支持(以及 GDB 支持),我可能不应该感到惊讶。事实上，Arduino IDE 就是这么刷机板的。这应该是显而易见的，因为该板实际上只是已经支持的 SAM D21 芯片的突破。

重复这是一个突破板的想法，我们认为他们做得很好。有两个 USB 接口；一个让您作为设备或主机访问电路板，而另一个连接调试硬件。如果你以前从未使用过片上调试器，它会改变你的生活，所以一定要试一试。当你通过了项目的初始原型阶段，你仍然可以使用 Zero 作为调试工具。有一个未组装的 10 引脚接头(不确定小间距接头是否附带)，可用于与目标板接口。[Bob]还花了一些时间讨论了可配置的 6 引脚接头，它允许您从一系列硬件协议(SPI、TWI 等)中进行选择。).

不幸的是，我们仍然没有关于供货时间表或价格信息的信息。这种预生产运行有一个小问题(PCB 上交换了两个信号)，他们需要旋转另一个电路板，进行填充和 QA，然后才能为最终产品开绿灯。

编辑注释: Atmel 在 Hackaday 上做广告，但这个视频和帖子不是这种关系的产物。Hackaday 不发布付费内容。

[https://www.youtube.com/embed/SxpscquBIo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SxpscquBIo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)