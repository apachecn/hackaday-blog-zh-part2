# 青少年音频图书馆

> 原文：<https://hackaday.com/2014/09/30/the-teensy-audio-library/>

有几种玩法。WAV 文件，但除此之外，进行任何严肃的音频处理都需要更强大的处理器。现在情况不同了:[Paul Stoffregen] [刚刚发布了他的 Teensy 音频库](http://www.pjrc.com/teensy/td_libs_Audio.html)，这是一个为 Teensy 3 中的 ARM Cortex M4 创建的库，它可以在 CD 质量的音频中进行 WAV 回放和录制、合成、分析、效果、过滤、混合和内部信号路由。

这是一段令人印象深刻的代码，因为 Teensy 3.1 中的 ARM Cortex M4 DSP 指令才成为可能。它不能在 8 位微处理器上运行，甚至不能在基于 M3 皮层的 Arduino 上运行。这是一个为青少年设计的项目，尽管[Paul]已经开源了所有的东西，并把它放到了 Github 上。还有一个[小巧的音频适配器板，配有一个 microSD 卡座、一个 1/8”插孔和一个麦克风连接器。](http://www.pjrc.com/store/teensy3_audio.html)

除了音频录制和回放，还有一个很棒的 FFT 对象，可以将你的音频频谱分成 512 个频段，以 86Hz 更新。如果你想要一个声音反应 LED 项目，有你去。还有相当多的正弦、锯齿、三角形、方形、脉冲和任意波形的合成功能，一些合唱、镶边、包络滤波器的效果功能，以及一个 [GUI 音频系统设计工具](http://www.pjrc.com/teensy/gui/)，它将代码直接输出到 Arduino IDE，以便上传到 Teensy。

这真的是令人难以置信的工作量，随着功能的增加，我们可以很容易地看到自制乐器的质量在接下来的几个月里大幅提高。这个东西有 DIY Akai MPC/单体，伪模拟合成器，或便携式效果盒写满了它。