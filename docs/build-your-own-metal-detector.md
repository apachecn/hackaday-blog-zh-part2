# 制作您自己的金属探测器

> 原文：<https://hackaday.com/2013/07/25/build-your-own-metal-detector/>

[Dzl]和他看起来相当严肃的儿子是金属探测器爱好者。但是今年夏天早些时候，当他们找不到从商店买来的金属探测器时，他们就自己动手做了一个。[Dzl]首先解释了大多数基于振荡器的金属探测器的工作原理。这款的不同之处在于[使用 Arduino 从金属探测线圈](http://dzlsevilgeniuslair.blogspot.dk/2013/07/diy-arduino-based-metal-detector.html)中读取数据。

电路从一个产生约 160 kHz 信号的振荡器开始，Arduino 不断测量该信号。当金属进入线圈时，它会改变频率，Arduino 会立即接收到该频率。这个装置使用压电蜂鸣器，发出你通常会联想到盖革计数器的那种滴答声，而不是那种特有的升调。

构建的最后一部分是找到最佳线圈方向。他们决定绕着一个金属桶转三十圈。一盏旧的宜家灯具是摆放他们的硬件的完美选择，看起来很有魅力。