# 8 引脚 AVR 上的仿真 ARM

> 原文：<https://hackaday.com/2012/04/17/emulating-arm-on-an-8-pin-avr/>

[![](img/ff7b7b37951d2256d4701458a7318ec4.png "attiny")](http://hackaday.com/wp-content/uploads/2012/04/attiny.png)

紧随其后的是一些精彩的“让我们看看我们可以在 AVR 上仿真什么”构建，我们已经看到，[Dimitri] [在 8 针 ATtiny85 上仿真了 ARM Cortex-M0](http://dmitry.co/index.php?p=./04.Thoughts/08.%20uM0) 。

仿真器完全是用 AVR 汇编写的。不幸的是，ATtinys 的指令集没有乘法指令，所以必须在单独的代码段中模拟。即使添加了这个，模拟器也非常小；内核只有 1300 多条指令，小到可以放在非常小的“tiny85”的闪存上。

与我们上个月看到的运行 Linux 的 ATMega 不同，[Dimitri]不会做任何疯狂的事情，比如制造有史以来最小最差的 Linux 电脑。M0 没有内存管理单元，所以 Linux 是不可能的。【迪米特里】可以用 [μCLinux](http://www.uclinux.org/status/) ，再加上一个 I2C EEPROM 和 RAM，但是不要指望一个速度为 200kHz 的仿真 ARM 会有速度恶魔。

[Dimitri]把所有的代码放在他的网页上，安装程序就可以运行了。它看起来很容易快速启动并运行，所以我们确信一些无聊的硬件专家会用这段代码做一些有趣的事情。