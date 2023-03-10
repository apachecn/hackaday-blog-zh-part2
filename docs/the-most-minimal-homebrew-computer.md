# 最小的自制电脑

> 原文：<https://hackaday.com/2013/10/21/the-most-minimal-homebrew-computer/>

完美不是在没有更多可以添加的时候实现的，而是在没有什么可以失败的时候实现的。按照这个标准，[【Stian】的三芯片 6502 自制电脑](http://jmp.no/blog/3-chip-computer)是完美的缩影。这是一台真正的、工作的、自制的逆向计算机，只使用了三个芯片:一个 CPU、一些 RAM 和一个微控制器来引导计算机并提供视频输出，

这种极简构建的关键是由 ATMega16 微控制器控制整个启动过程，该微控制器通过双端口 SRAM、[1 千字节 Cypress CY7C130](http://www.cypress.com/?mpn=CY7C130-55PC) 与 6502 接口。这种双端口 RAM 允许 CPU 和微控制器访问相同的内存位，从而很容易从一位 AVR 代码启动计算机。

输出由[Stian]的 [ATMega 视频文本发生器](http://jmp.no/blog/amvtg/)提供，将 37×17 字符放在任何带有 RCA 插孔的电视机上。虽然输入还没有被处理，[Stian]说用他的 [AVR PS/2 键盘库](http://jmp.no/blog/atps2key/)应该可以做到。

虽然其他 6502 自制电脑如[【Quinn Dunki】Veronica](http://hackaday.com/2013/02/25/veronica-6502-computer-reaches-hello-world-stage/)可以达到无与伦比的复杂程度，但关于[Stian]的三芯片电脑的极简主义还有很多可说的。通过一些巧妙的编码和修改过的零件清单，很有可能以最低的成本和最少的零件把一台改装计算机送到每个人的手中。