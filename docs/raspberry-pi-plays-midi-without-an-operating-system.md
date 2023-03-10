# 树莓派在没有操作系统的情况下播放 MIDI

> 原文：<https://hackaday.com/2013/01/22/raspberry-pi-plays-midi-without-an-operating-system/>

[https://www.youtube.com/embed/k6TCysv6AzE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/k6TCysv6AzE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

对于树莓 Pi 中锁定的所有有趣的 DSP 功能，仍然很难想象使用树莓 Pi 作为一个非常强大的软件合成器、跟踪器或序列器。运行任何常见的 Linux 数字音频程序都意味着——令人惊讶地——运行 Linux，以及与之相关的性能损失。

如果所有这些音频程序都可以在没有操作系统的情况下直接在 Raspberry Pi 上运行，那会好得多，而[Joe]的项目就在这条路上。[他在没有操作系统的情况下播放 MIDI 文件，](http://www.joebutton.co.uk/blog/baremetal-midi-lv2-raspberrypi/)实际上使 Raspberry Pi 成为一个非常强大的嵌入式平台。

[Joe]的构建是 Raspberry Pi 的第一个裸机音频代码。它实际上是一个 [LV2](https://en.wikipedia.org/wiki/LV2) 插件主机，将加载音频插件，读取 MIDI 文件，并通过 Pi 上的 1/8”插孔输出结果音频。如果没有[大卫·韦尔奇]整理的一些[树莓派裸机教程](https://github.com/dwelch67/raspberrypi)，这项工作是不可能完成的。

希望这不会是我们最后一次看到[Joe]和他的代码；树莓派有足够的马力成为一个惊人的采样器，合成器，打击机，或下一代的 Akai MPC。我们所需要的只是一些勇敢的编码员在树莓派上开始编码裸机。