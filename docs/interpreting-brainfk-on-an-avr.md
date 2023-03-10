# 在 AVR 上解释 Brainf*#k

> 原文：<https://hackaday.com/2013/02/27/interpreting-brainfk-on-an-avr/>

我们不会说它没用，但我们会问为什么[Dan] [为 AVR](http://eds.dyndns.org/~ircjunk/tutorials/prog/avrbf/main.html) 写了一个 brainfuck 解释器

它没有为 AVR 生成代码；更像是一个引导加载程序。为了运行 brainfuck 程序，[Dan]将其上传到他的 ATMega32 内部的 EEPROM 中，之后微控制器接管并开始执行 brainfuck 程序告诉它做的任何指令。因为整个过程是在 EEPROM 上运行的，所以代码大小被限制在 1022 字节以内。我们认为，对于人类写的任何脑残程序来说都足够了。

至于为什么[丹]想要一个 AVR 来为一种人类几乎无法理解的语言建立一个解释器，老实说，我们除了普遍的“因为它在那里”的情绪之外没有任何想法。有一些非常酷的项目使用 brainfuck，包括遗传算法软件开发商。不过，现在，blinkey LEDs 足以让我们开心，所以你可以在休息后在 LED 显示屏上看到 brainfuck 的视频。

[https://www.youtube.com/embed/B9p9-3T_TnI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/B9p9-3T_TnI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)