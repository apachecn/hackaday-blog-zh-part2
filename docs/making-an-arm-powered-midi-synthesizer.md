# 制作 ARM 供电的 MIDI 合成器

> 原文：<https://hackaday.com/2013/12/28/making-an-arm-powered-midi-synthesizer/>

[![](img/7fbc4977279b2fb7269af7485f6d173f.png)](http://hackaday.com/wp-content/uploads/2013/12/xxx.jpg)

你在上面的图片中看到的是一个手工制作的 [4 振荡器合成器](https://github.com/74hc595/LPC1114-Synthesizer)，带有 MIDI 输入、多模式滤波器和少量调制选项。它是由[Matt]建造的，他是一个习惯了 AVR 的电子爱好者，为了这个项目，他打破了自己的习惯。该平台的核心是一个 DIP 封装的 32 位 Cortex-M0 ARM 处理器(LPC1114)，其中填充了“手动”编写的汇编代码和编译的 C 函数。在 50MHz 时钟速度下，微控制器可以在 12 位 DAC 上输出 250kHz 的样本，同时由 3 节 AA 电池供电。

阅读[Matt]的文章，我们发现他创建的固件使用 4 个振荡器(锯齿或脉冲形状)和一个低频振荡器(三角形、斜坡、正方形、随机形状)。它还包括一个 2 极[状态变量滤波器](http://en.wikipedia.org/wiki/State_variable_filter)和调整攻击-释放包络的能力(等等)。系统从连接的设备获取 MIDI 命令。休息之后，我们嵌入了他创作的视频。

[https://www.youtube.com/embed/DU8IyjyjDfk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DU8IyjyjDfk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/o-3MleRX-aE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/o-3MleRX-aE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)