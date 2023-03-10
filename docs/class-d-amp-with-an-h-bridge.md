# 带 H 桥的 D 类放大器

> 原文：<https://hackaday.com/2014/12/28/class-d-amp-with-an-h-bridge/>

D 类放大器很简单，只需输入一个信号，用 PWM 调制一个方波。将这个 PWM 信号发送到一个 MOSFET 或其他器件，你就拥有了最简单的 D 类放大器。它们非常简单，你可以花 3 美元买一个 D 类放大器芯片，但[乔治]认为这太容易了。相反，他用 ATTiny 和 H 桥电机驱动器建造了自己的汽车。毫不奇怪，它是有效的，但有趣的是 ATtiny 上的代码会对扬声器输出的音频质量产生什么影响。

这个项目选择的微控制器是 ATtiny 461，这是一个我们不常见到的器件，但仍然是你对 ATtiny 的期望。这个构建中最重要的部分是在易贝花几美元买到的 L298 芯片。这种双 H 桥通常用于驱动电机，但[George]在放大器的功率部分为它找到了一个家。

ATtiny 的时钟频率为 16 MHz，因此 ADC 的时钟频率为 1 MHz。发生 10 位精度转换，该值设置 PWM 占空比。芯片中的定时器 1 设置为 32 MHz，通过将该定时器计数到 1023，该放大器的 PWM 周期速度为 31.25 kHz。这正好是 D 类放大器应该运行的速度，代码只有大约 30 行。没有比这更简单的了。

[George]放了一个这个放大器工作的视频，[尽管没有遵循 D 类放大器](http://hackaday.com/2014/06/09/afrotechs-guide-to-class-d-amplifiers/)的标准设计，但听起来相当不错。你可以看下面的视频。

[https://www.youtube.com/embed/YnEALQKMY4A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YnEALQKMY4A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)