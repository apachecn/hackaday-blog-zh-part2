# 树莓派席德播放器

> 原文：<https://hackaday.com/2015/02/06/a-raspberry-pi-sid-player/>

在所有的老式 chiptune 机器中，Commodore 64 是最著名的。即使 30 年后，仍然有大规模的聚会致力于从 CPU 和臭名昭著的片上合成器 SID 中寻找最后一个周期的处理能力和图形能力。[鲍勃]想建立一个 SID 点唱机。C64 能够胜任这项工作，但是如果你想在 SD 卡上拥有所有的 SID 成分并将其连接到网络上，[Raspberry Pi 是一个不错的选择](http://www.acsu.buffalo.edu/~robertsz/projects/SID/index.html)。

6581 或 8580 版本的 SID 芯片是通过地址和数据总线拨动芯片上的寄存器来直接控制的。这意味着很多引脚，对于原来的 Raspi 扩展接头来说太多了。不过，这不是一个用几个移位寄存器就能解决的问题。电路的其余部分是一个 LM386 音频放大器、一个显示当前歌曲的 LCD 和一个用于 SID 的 can 晶体振荡器。

现在一切都在试验板上，但是做一个树莓帽会是一个相当简单的提议。这只是找到一个具有有效过滤器的 SID 的问题，如果您能做到这一点，那么复制它就相当容易了。下面视频。

[https://www.youtube.com/embed/up9tZVzffEo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/up9tZVzffEo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)