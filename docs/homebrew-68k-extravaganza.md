# 家酿 68k 盛会

> 原文：<https://hackaday.com/2012/09/04/homebrew-68k-extravaganza/>

[![](img/563297bbcb1b8db3d2738b2748d9a175.png "68k")](http://www.cpu-world.com/CPUs/68000/)

摩托罗拉 68000 CPU T1 于 1979 年推出，最初用于 Sun 和 SGI 等非常昂贵和非常高端的工作站。随着处理器的成熟，它因在最初的 Macintosh、早期的 Amigas，甚至 TI-89 图形计算器和一些视频游戏控制台(如 Sega Genesis 和 Atari Jaguar)中的使用而闻名。

几天前，当我发布了一个基于 65816 CPU 的自制电脑版本时，我感叹缺乏使用古老的摩托罗拉 68k 的版本。Hackaday 的读者很快就指出了许多自制电脑使用这种经典的 CPU，我很高兴在这里张贴它们。

首先是[一个令人惊叹的 68008 版本](http://www.youtube.com/watch?v=Q7Wmt7UEXtc)，它具有 IDE 磁盘接口、软盘接口、10base-T 以太网连接、实时时钟和*两个* SID 合成器芯片。就功能而言，这个版本是最棒的。可惜我找不到相关报道。

这里有一台基于 68000 的计算机围绕 S-100 总线构建。像第一台使用 S-100 总线的计算机 [Altair 8800](http://en.wikipedia.org/wiki/Altair_8800) 一样，这台计算机被插入一个背板，该背板将数据、地址和中断线路分发给总线上的每个设备。

当然，如果没有 Eurocard 版本，提到背板计算机是不完整的。[N8VEM] [建造了一台 68000 计算机](http://n8vem-sbc.pbworks.com/w/browse/#view=ViewFolder&param=ECB%20mini-M68000)，它能够与 IDE 控制卡和[显示控制器](http://n8vem-sbc.pbworks.com/w/file/48864748/babyM68k%2Bdisplay.JPG)一起插入背板。

最后，本着真正的“电线的巨大混乱”精神，[Dajgoro]送来了他的 68k 单板计算机，具有 512 kB 的 RAM 和 16k 的 ROM。[Dajgoro]还花时间连接 PIC 微控制器，使他能够扩展他的计算机，远远超出老式组件所允许的范围。

68k 过去是，现在仍然是非常强大的 CPU，远远超过我们不时看到的 6502 和 Z80 自制计算机的能力。除了从零开始构建基于 486 或奔腾的计算机之外，构建 68k 机器是硬件黑客的最高成就之一，也是我们希望在未来看到更多的成就。