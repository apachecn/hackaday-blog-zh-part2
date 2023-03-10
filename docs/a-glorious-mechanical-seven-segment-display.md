# 辉煌的机械七段显示器

> 原文：<https://hackaday.com/2012/04/15/a-glorious-mechanical-seven-segment-display/>

如果你曾经想知道为什么你从来没有见过机械七段显示器，[现在你知道](http://www.schoar.de/tinkering/sevenblocks/)了。它们相当复杂，而且很可能贵得离谱，尤其是当几个灯泡或发光二极管同样能做好同样的工作时。这并没有阻止[kiu]完成他称之为 SevenBlocks 的机械七段钟，为此我们心存感激。

[kiu]时钟的 28 个部分中的每一个都由三层丙烯酸树脂和一小段齿条制成。与你见过的每一个七段显示器不同，[微小的业余爱好伺服系统](http://www.hobbyking.com/hobbycity/store/uh_viewItem.asp?idProduct=663)为每一段提供指示。对于电子设备，ATMega8 用于装备的大脑，74HC595 移位寄存器用于扩展 I/O 线的数量。DS1307 RTC 模块提供精确的计时，在“guts shot”中可见的几十个伺服输出让你意识到为什么你以前从未见过机械七段显示器——它们真的很复杂。

如果你想打造自己的机械七段钟，[kiu]把[所有文件放到 Github](https://github.com/kiu/SevenBlocks) 上。一切都在那里，从。DXF 文件准备好输入激光切割机，为三个 PCB 中的每一个提供原理图和电路板文件。展示这个时钟运行的视频是必要的，所以你可以在休息后看看。

[https://www.youtube.com/embed/H2ZiZt0TA9A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H2ZiZt0TA9A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)