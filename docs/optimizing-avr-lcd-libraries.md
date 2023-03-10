# 优化 AVR LCD 库

> 原文：<https://hackaday.com/2015/06/01/optimizing-avr-lcd-libraries/>

不久前，Teensy 系列微控制器的创造者[Paul Stoffregen]利用最流行的 Arduino 库来驱动 TFT LCDs。Teensy 不是 Arduino——它要快得多——但是[Paul]的库做任何事情都更有效率。

即使使用标准的 Arduino，在驱动 TFT 时仍然可以提高速度和效率。[Xark] [最近发布了他的 Adafruit GFX 库和 LCD 驱动程序的重新组合](https://hackaday.io/project/6038-pdqgfx-optimzed-avr-lcd-graphics)。它比 Adafruit 库快好几倍，所以如果你还没有在 Teensy 平台上移动，这是使用这些重新利用的手机显示器的方法。

在阅读了[Paul]为青少年改进 TFT 库的经验后，[Xark]拿起一个 Arduino、一个 LCD 和一个开放式工作台逻辑嗅探器来查看 Adafruit 库中效率低下的地方。这些显示器通过 SPI 驱动，当数据线上的每个字节移出时，时钟信号变为低电平。对于 Adafruit 库，每个时钟信号之间会浪费大量时间，如果代码正确，性能可以得到显著提高。

[关于[Xark]如何改进这些显示器的代码的文章](https://hackaday.io/post/18729)非常精彩，结果令人印象深刻；他可以以大约 13FPS 的速度在屏幕上填充像素，使任何时候都不会重绘太多屏幕的游戏成为现实。