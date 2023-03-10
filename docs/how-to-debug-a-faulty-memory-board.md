# 如何调试有故障的内存板

> 原文：<https://hackaday.com/2013/08/09/how-to-debug-a-faulty-memory-board/>

[![ram](img/10c57db1708ed7225d267bd8f6ff1fc1.png)](http://hackaday.com/wp-content/uploads/2013/08/ram.jpg)

虽然这不完全是一次黑客攻击或失败，但它绝对是一个关于如何调试一个有问题的卡的鼓舞人心的例子。

[Quinn]是少数几个自己设计基于 6502 的计算机的爱好者之一。对于 Hackaday 的年轻读者来说， [MOS 6502](https://en.wikipedia.org/wiki/MOS_Technology_6502) 于 1975 年推出，并已用于 Aple //系列、Commodore 64、Vic-20、Atari 计算机、任天堂 Enterntainment 系统等。

[Quinn]的自制的 新 RAM 板已经工作了许多周，直到它开始显示出一些弱点，只是偶尔通过引导 RAM 测试。假设 RAM 是问题所在，她开始做一个更高级的内存测试，显示随机地址的错误。

她手头已经没有同样的内存芯片可以和新的 PCB 一起使用了。她决心解决这个问题，在一块新的主板上蚀刻了新的内存设计。不幸的是，它还会在启动时出现内存错误。只剩下一个罪魁祸首，如上图所示。这是电路板图形中的一个小尺寸误差，足以导致连接器错位。

这篇文章包含了许多关于她的调试过程的细节，所以绝对值得一读。