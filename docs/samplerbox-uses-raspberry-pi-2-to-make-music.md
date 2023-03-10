# SamplerBox 使用 Raspberry Pi 2 制作音乐

> 原文：<https://hackaday.com/2015/06/12/samplerbox-uses-raspberry-pi-2-to-make-music/>

[JosephErnest]想要一种经济高效的替代方案来替代市场上可买到的 MIDI 采样器和扩展器。他还想避免一直被电脑束缚。他的解决方案是[sample box](http://www.samplerbox.org/)，这是一款独立的即插即用采样器，制作成本不到 100 欧元。只需插入一个 SD 卡与你的 WAV 格式的样本集，启动它，并通过您的键盘或 MIDI 控制器发挥你的心的内容！

[JosephErnest]在 SamplerBox 中使用了 Raspberry Pi 2，因为它提供了更高的性能。他对其内置声卡的音质不太满意，所以他安装了一个 USB DAC [PCM2704](http://www.ti.com/product/pcm2704) (一个旧型号，但任何 USB DAC 都可以)来输出音频。他还安装了一个 USB 读卡器，以便更容易地切换包含采样器集的 SD 卡，同时保持 Pi 2 自己的 microUSB 卡专用于操作系统和软件。DIN MIDI 连接器和 USB 都作为 MIDI 输入包含在设计中。如果您只打算使用 USB，MIDI 连接器可以从构建中省略。[软件是用 Python 和](https://github.com/josephernest/SamplerBox) [cython](https://github.com/josephernest/SamplerBox) 编写的，这使得 Pi 2 可以拥有超过 128 种声音的复调。用户也可以创建他们自己的样品组来使用 SamplerBox。预设更改可以在运行中进行。我们所需要的只是一些音乐课！

[https://www.youtube.com/embed/CDJ87UMOsE8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CDJ87UMOsE8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/raspberry_pi/comments/36heu2/raspberry_fields_forever_strawberry_pi/)