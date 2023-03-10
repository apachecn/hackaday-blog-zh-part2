# 用于 GLCD 屏幕的双线串行背包

> 原文：<https://hackaday.com/2013/03/11/two-wire-serial-backpack-for-glcd-screens/>

[Debraj]写了他为图形 LCD 屏幕开发的[双线串行背包](https://sites.google.com/site/hobbydebraj/home/2-line-interface-for-graphic-lcd)。它建立在一大块原型板上，使用一对 595 移位寄存器将输入的串行数据转换为 LCD 屏幕使用的并行接口。以这种方式推送命令需要更多的时间，但是你可以在跳转后的剪辑中看到，界面仍然很快。

这里真正的诀窍是硬件是如何配置的，没有第三根线来锁存移位寄存器(如果你需要 595 芯片的入门知识[请查看这个功能](http://hackaday.com/2011/11/05/controlling-shift-registers-via-spi/))。使用锁存器的想法是，在数据出现在输出引脚之前，所有数据都可以通过串行引脚移入。否则，GLCD 会在每个位移入寄存器时看到它，从而严重破坏其通信协议。[Debraj]通过使用他从另一个系列 LCD 项目中学到的[二极管和栅极技巧来解决这个问题。](https://code.google.com/p/arduinoshiftreglcd/#With_diode-resistor_AND_gate)

这种方法的一个好处是 595 芯片具有宽范围的控制电压，允许您使用 3.3V 或 5V 微控制器来驱动它。但是您确实需要实现通信协议，并通过串行发送这些命令。在几乎相同的芯片成本下，可以用类似 ATtiny2313 的东西来替代，以实现更简单的寻址方案，甚至切换到 1 线协议。但这样会失去宽输入电压容差。

[https://www.youtube.com/embed/XqOWdbxRCaY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XqOWdbxRCaY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)