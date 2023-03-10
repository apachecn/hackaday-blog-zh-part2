# 一种可黑客攻击的高保真音频 DSP

> 原文：<https://hackaday.com/2014/08/20/a-hackable-hi-fi-audio-dsp/>

[![DSP 01 Hi-fi Signal Processor](img/b2b3a02b25ec5d2100e3cb866b01cc79.png)](http://hackaday.com/2014/08/20/a-hackable-hi-fi-audio-dsp/dsp01/)

音响发烧友倾向于把模拟系统放在基座上。模拟系统可以提供出色的音频性能，但往往价格不菲。它们也很难修改，因为修改参数需要更换组件。为了解决这个问题，[tshen2]设计了 [DSP 01](http://hackaday.io/project/2374) 。

DSP 01 基于 ADI 公司的 ADAU1701。该 DSP 芯片包括两个用于音频输入的 ADC 和四个用于音频输出的 DAC。这些可以由内置的 DSP 处理器内核控制，该内核具有用于开关、按钮和旋钮的 I/O。

DSP 01 的主要目标是实现[音频交叉](http://en.wikipedia.org/wiki/Audio_crossover)。该设备接收输入音频信号，并根据频率对其进行分割，以便低音炮获得低频成分，高音喇叭获得高频成分。这对于良好的音频性能至关重要，因为驱动器只能在音频频谱的特定部分表现良好。

ADI 公司提供 [SigmaStudio](http://www.analog.com/en/dsp-software/ss_sigst_02/sw.html) ，这是一款免费工具，您可以通过拖放界面对 DSP 进行编程。通过放入一些元件并对 EEPROM 进行编程，DSP 可以针对各种应用轻松进行重新配置。