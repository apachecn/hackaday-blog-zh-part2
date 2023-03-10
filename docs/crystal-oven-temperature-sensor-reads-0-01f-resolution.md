# 晶体炉温度传感器读数分辨率为 0.01F

> 原文：<https://hackaday.com/2013/06/19/crystal-oven-temperature-sensor-reads-0-01f-resolution/>

![crystal-oven-temperature-sensor](img/e0d57b804a41cec20ffbb0bf00214ce7.png)

[斯科特·哈登]继续他在高精度水晶炉上的工作。能够设定精确的温度取决于精确测量温度的能力。这就是这个电路的由来。它基于 LM335 线性温度传感器。他设计了支持电路，可以以百分之一度的分辨率读取温度。

用 AVR 微控制器的模数转换器(ADC)直接读取传感器只会产生大约 1-2 度的范围。他通过将传感器的输出放大到特定的范围来解决这个问题。为了演示，他将摆幅从 0-5V 调整到室温到体温范围。

当然，他使用模拟电路来实现这一点。但是在我们的纯数字读者点击离开之前，你应该看看他的视频解释。这展示了运算放大器的基本功能。我们认为[Scott]通过提供清晰易读的示意图和缓慢完整地解释每一部分，在介绍概念方面做得很好。

那么我们提到的这个水晶烤箱是什么呢？这是几年前的一个广播项目。

[https://www.youtube.com/embed/LTPncC2e3Zo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LTPncC2e3Zo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)