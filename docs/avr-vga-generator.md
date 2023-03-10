# AVR VGA 发生器

> 原文：<https://hackaday.com/2013/03/29/avr-vga-generator/>

![avr-vga-generator](img/a1b9564fef1e2b7837afb1ab3c07db13.png)

这个简单的电路构成了基于 AVR 的 VGA 发生器的硬件。他设法让 ATmega1284 输出稳定的 VGA 信号。任何研究过 VGA 标准的人都会知道这是一项了不起的成就。这是因为 VGA 是关于时间的，这几乎立刻给他带来了一个问题。

该芯片的最高运行速度为 20 MHz。[Andrew]成功编写了代码，实现了这种速度下的水平和垂直同步。但是没有足够的时钟周期来处理帧缓冲。他的解决方案是将芯片超频到 25 MHz。我们假设他选择这个是因为他手头有一个晶体，因为我们认为使用 25.174 MHz 晶体会更容易，这是规格中列出的速度之一。

红色、绿色和蓝色各自通过一组电阻选择各自的两位范围，总共 64 种颜色。正如您在休息后的视频中看到的，128×96 像素的视频已经启动并运行。[Andrew]计划从这里开始扩大项目的范围，使其比仅仅显示标准图像更加多样化。代码(用汇编语言编写)可以在[他的 GitHub 库](https://github.com/aarossig/avr-vga)中获得。

[https://www.youtube.com/embed/YHREZeoF7Tk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YHREZeoF7Tk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)