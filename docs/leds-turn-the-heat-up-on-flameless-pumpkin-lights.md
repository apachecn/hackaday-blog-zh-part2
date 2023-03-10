# 发光二极管打开无焰南瓜灯的热量

> 原文：<https://hackaday.com/2013/10/01/leds-turn-the-heat-up-on-flameless-pumpkin-lights/>

![led-peter](img/3db45812df050da229023c0e55c956a2.png)

当茶灯不行的时候，为什么不升级到一个 [5 通道 LED 蜡烛模拟器](http://www.wire2wire.org/LED_candle/LED_candle.html) [r](http://www.wire2wire.org/LED_candle/LED_candle.html) ？

万圣节快到了。彼得当地的黑客空间兔子洞(Rabbit Hole)有一个雕刻南瓜和讨论万圣节黑客的会议。在看到一盏茶灯对一个中等大小的南瓜的照明有多差后，这个黑客就诞生了。我们以前见过 [LED 鬼火黑客](http://hackaday.com/2008/10/21/flameless-jack-o-lantern-with-an-attiny13/)，但这一次值得再看一眼。

按照真正的黑客空间风格，[彼得]利用了他所能得到的一切。一张 PIC12F508 是该项目的心脏。12X508/9 系列已经存在了很多年，仍然是一款很好的芯片。我们记得使用这种芯片的“C”版本来绕过原始 PlayStation 系统上的区域锁定。[Peter]创建了一个具有两种基本模式的简单电路。在“值模式”下，508 直接从其 I/O 引脚驱动 LED。这将总输出限制在 60mA。在“高级模式”下，一些 2N3904 NPN 晶体管用于处理电流。这允许 PIC 驱动多达 5 个 led。

用 led 模拟蜡烛可能会很棘手。【Peter】使用 5 个独立的 16 位[线性反馈移位寄存器](http://en.wikipedia.org/wiki/Linear_feedback_shift_register)产生[伪随机比特流](http://en.wikipedia.org/wiki/Pseudorandom_number_generator)。效果相当可观。一个“风的模拟”完成了真实火焰的幻觉。

微处理器的一个引脚用于在超值模式和高级模式之间切换。我们希望看到的一种模式是收回 I/O 引脚，并将其连接到风传感器，可能是麦克风或气流传感器。使用传感器触发风模式，获得更真实的蜡烛模拟。

[https://www.youtube.com/embed/dPsVr4pU8Tg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dPsVr4pU8Tg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)