# 以模拟方式构建音频频谱分析仪

> 原文：<https://hackaday.com/2014/01/03/build-an-audio-spectrum-analyzer-the-analog-way/>

![bandpass](img/8954cb3cba8481ad39e46ebff7c1353d.png)

[Ryan]想要为他的音频设备安装一个频谱分析仪。他用模拟的方式做了这件事，而不是用微处理器。[Ryan]设计了一个 10 波段音频频谱分析仪。这意味着他需要 10 个带通滤波器。顾名思义，[带通滤波器](http://en.wikipedia.org/wiki/Band-pass_filter)将只允许所选频段频率的信号通过。频率高于或低于滤波器通带的信号将被衰减。带通本身由高通和低通滤波器构成。[Ryan]使用简单的电阻电容(RC)滤波器来实现他的设计。

所有这些分立元件都会迅速衰减[Ryan 的]输入信号，因此每一级使用两个运算放大器。第一级是每个频带的缓冲器。位于带通滤波器之后的第二个运算放大器被配置为[同相放大器](http://en.wikipedia.org/wiki/Operational_amplifier#Non-inverting_amplifier)。这些放大器在单个频段信号离开电路板之前对其进行增强。[Ryan]甚至增加了一个“能量填充”模式。在正常模式下，分析仪的输出将完全跟随输入信号。在“能量填充”(又名峰值检测)模式下，输出将显示信号峰值，并缓慢衰减至输入信号。能量填充模式通过使用 n 沟道 FET 在电解电容中存储电荷来创建。

我们是否提到过，对于 10 个频段，所有这些电路必须构建 10 次？更不用说输入缓冲电路了。完成所有这些工作后，[Ryan]还需要构建分析仪的输出部分:160 个蓝色发光二极管及其相关的驱动电路。在今天这个高速微控制器和 FFT 的时代，“全模拟”可能看起来很疯狂，但简单的事实是，这些电路工作，而且工作得很好。唯一需要担心的是 perf 板焊接短路。我们认为调试这些是乐趣的一半。