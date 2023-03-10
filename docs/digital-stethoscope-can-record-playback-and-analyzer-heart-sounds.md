# 数字听诊器可以记录、回放和分析心音

> 原文：<https://hackaday.com/2012/05/11/digital-stethoscope-can-record-playback-and-analyzer-heart-sounds/>

![](img/5e15496da6be43fab1c2b2b456b1651b.png "stethoscope_box2")

这些相当便宜的电子设备如何能够增强普通听诊器的功能，这有点令人惊讶。这种数字听诊器使用音频处理来增加功能。一个标准的胸式话筒为电容话筒供电，电容话筒通过一个非常标准的运算放大器电路供电，运算放大器电路为 ATmega644 的 ADC 供电。数字化后，心音可以以 10 秒的增量记录到 1 Mb 的闪存芯片中。数据也可以通过 USB 电缆实时输入 MATLAB。在那里，它显示为一个波形，并在飞行中计算心率。休息之后，请观看该系统的精彩演示视频。

上图是一组用作输出的耳塞。但这是一个标准的耳机插孔，所以心音可以在扬声器上播放，我们认为这对于教学来说会很方便。如果医生不在附近，还可以选择将它连接到计算机输入，这可能是用于 Skype 会话的音频。这里有很大的潜力，而且成本相当低，我们喜欢这样！

[https://www.youtube.com/embed/i_iY8ARsrvQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/i_iY8ARsrvQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)