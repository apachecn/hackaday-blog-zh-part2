# 构建软件定义的无线电

> 原文：<https://hackaday.com/2014/04/25/building-a-software-defined-radio-with-a-teensy/>

[Rich，VE3MKC]想进入软件无线电已经有一段时间了，但不想走通常的 PC 路线。他最初认为 Raspberry Pi 将是可以操纵音频的小型嵌入式设备的最佳平台，但在发现 ARM 驱动的 Teensy 3.0 之后，[有了一个完全不同的项目。](http://rheslip.blogspot.ca/2014/04/software-defined-radio-with-teensy-31.html)

[Rich]正在使用一个 [SoftRock SDR](http://softrocksdr.wikispaces.com/) 从天线获取 RF，并将其下变频到音频范围。为 SDR 做 DSP 是相当计算密集型的，但是他发现一个带有[音频适配板](http://www.pjrc.com/store/teensy3_audio.html)的 Teensy 3.0 可以胜任这项任务。

到目前为止，[Rich]正在将音频从 SoftRock 传输到 Teensy，在那里音频被数字化并乘以 VFO，通过滤波器发送，然后发送到耳机插孔的输出端，再到扬声器。音频适配器板上的音量壶用于调节 VFO，将来某个时候会被合适的编码器取代。

在下面的视频中，你可以看到[Rich]正在收听一场比赛，一个小小的 TFT 显示屏显示每个人都在直播。这是一个非常酷的构建，即使它仍然处于开发的早期，对于青少年来说，仍然有大量的 CPU 周期来做一些非常酷的事情。

[https://www.youtube.com/embed/9pZnqMBpSdc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9pZnqMBpSdc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Jjm9rANNi1o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Jjm9rANNi1o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)