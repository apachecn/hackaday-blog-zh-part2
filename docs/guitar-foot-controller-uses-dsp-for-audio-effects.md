# 吉他脚控制器使用 DSP 实现音频效果

> 原文：<https://hackaday.com/2012/11/30/guitar-foot-controller-uses-dsp-for-audio-effects/>

![guitar-pedal-dsp1](img/251d49aa9a7bb80c3ede2850493037f1.png)

这是从[Pierre 的]结合 DSP 和纯数据的电吉他效果踏板演示中截取的截图。他通过将吉他直接连接到计算机上来实现这一点，然后将计算机的音频输出馈送到吉他放大器。

脚部控制包括一个踏板和八个按钮，都由 Arduino 监控。[纯数据](http://en.wikipedia.org/wiki/Pure_Data)，一种可视化编程语言，通过 USB 解释来自 Arduino 的输入，并使用数字信号处理改变输入的音频。[Pierre]使用[插孔音频连接套件](http://jackaudio.org/)软件包管理音频连接。

在休息后的视频中，他用笔记本电脑完成了大部分工作，但他也用树莓酱完成了这项工作。RPi 板上没有音频输入，但他一直用的是 USB 声卡。另一个 USB 端口连接 Arduino，他开始工作了。

[https://www.youtube.com/embed/6g1l9W9suWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6g1l9W9suWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢沃尔特]