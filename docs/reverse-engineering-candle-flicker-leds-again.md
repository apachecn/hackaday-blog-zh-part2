# 逆向工程蜡烛闪烁发光二极管，再次

> 原文：<https://hackaday.com/2014/03/02/reverse-engineering-candle-flicker-leds-again/>

如今，闪烁的蜡烛 led 似乎无处不在，就像所有的时尚一样，有人不得不[近距离观察它们背后的工程。](http://cpldcpu.wordpress.com/2014/03/01/follow-up-on-candle-flicker-leds/)

[cpldcpu]早些时候通过测量使用的电流和开发这些 led 如何闪烁的统计模型，研究了这些蜡烛闪烁 led 中的控制器芯片。这是数学，当然，更多的乐趣可以通过解封这些闪烁 LED 控制器芯片之一。这不是很先进的技术。LED 控制器使用 1 或 2um 工艺和一对 RC 振荡器，但似乎在该芯片的硅中有一个硬件随机数发生器。

早些时候，[Cpldcpu]已经查看了这些闪烁的 LED 中的微型控制器，并确定他们使用了[线性反馈移位寄存器](http://en.wikipedia.org/wiki/Linear_feedback_shift_register)来产生伪随机 LED 强度。新的拆卸似乎证实了线性反馈移位寄存器正被用于驱动闪烁的 LED。

定制芯片只是给猫剥皮或使 LED 闪烁的一种方式，PICatout 使用了[最小的 PIC 微控制器](http://picatout-jd.blogspot.ca/2013/12/led-scintillante.html)(法语，[翻译](http://translate.google.com/translate?sl=fr&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fpicatout-jd.blogspot.ca%2F2013%2F12%2Fled-scintillante.html&act=url))来创造他自己的闪烁 LED。看起来做几个定制的闪烁 LED 投掷器应该不会太难。