# 入门级难度的低级计算:DUO Light

> 原文：<https://hackaday.com/2014/09/20/low-level-computing-with-entry-level-difficulty-duo-light/>

硬件再简单不过了。DUO Light 使用 ATmega328(通常在 Arduino 板上找到)和外部 SRAM 芯片来提供低级计算机编程体验，这将适合编程新手和一些更有经验的修补者。

在撰写本文时，Kickstarter 的目标是 1100 美元，离成功只差 18 美元。我们敢打赌，这部分是由于[在【杰克的】网站上有如此多的支持材料](http://www.ostracodfiles.com/light/menu.html)。(仅供参考——该页面上的许多链接都是 zip 文件)

SD 卡插槽接受 FAT16 卡和程序字节码。可用的 Psuedo C 编译器和汇编器让你选择你的毒药，或者你可以简单地直接[钻研字节码](http://www.ostracodfiles.com/light/DLBC.txt)。我们没有看到原理图，但固件和 BOM 都是可用的。你应该能够很容易地找出其中的联系。

很长一段时间以来，我们一直是[杰克]作品的粉丝。他的 TTL 电脑 T1 和 T2 的 16 核 ATmega T3 肯定会让你高兴，即使你记得第一次看到它们的时候。这也不是他第一次尝试教育模式。尽管我们仍然发现[他的逻辑芯片计算机](http://hackaday.com/2013/11/03/duo-basic-an-all-logic-chip-educational-computer/)有点令人生畏。