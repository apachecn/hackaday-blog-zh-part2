# 学习移位寄存器而不涉及微控制器

> 原文：<https://hackaday.com/2013/02/07/learn-shift-registers-without-involving-a-microcontroller/>

这是一种真正的动手学习方法。[Kevin Darrah]抛弃了微控制器，正在使用按钮学习 595 个移位寄存器。测试设备使用两个串行输入并行输出芯片。这些是级联的，这意味着当来自第一个芯片的数据溢出时，它馈入第二个芯片的输入。这些部件通常用于驱动发光二极管，或者减少驱动外围设备[所需的引脚数量，比如这个字符 LCD](http://hackaday.com/2011/04/07/shift-register-is-all-it-takes-to-make-a-3-wire-serial-lcd/) 。

这五个按钮让你有机会直观地了解芯片逻辑是如何工作的。空白按钮通常也称为输出使能(OE)。将其驱动至高电平会关闭芯片输出，但不会清除数据。该任务由 clear 按钮执行，该按钮被拉低以将所有移位寄存器存储器设置为零。其他三个按钮设置逻辑电平，使用时钟信号将其移入芯片，并使用锁存器将存储的值推送到输出端。

为了直观地了解这些芯片内部的情况，你应该看看这篇文章中链接到[的移位寄存器教程。](http://hackaday.com/2011/11/05/controlling-shift-registers-via-spi/)

[https://www.youtube.com/embed/6fVbJbNPrEU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6fVbJbNPrEU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)