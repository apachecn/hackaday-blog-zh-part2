# 让[Euler]帮助 PCB 制造

> 原文：<https://hackaday.com/2013/01/11/letting-euler-help-out-with-pcb-fabrication/>

![drillin](img/c1350222b2f9ec1dab87c1445ad00501.png)

自从[阿莱西奥]开始蚀刻自己的印刷电路板，他发现了这个过程中最乏味的部分，自制 SMD 板如此棒的原因是:在自己的板上钻孔是一件痛苦的事。虽然[Alessio]的 CNC 工厂负责大部分工作，但对齐预钻孔板和纠正掩模的任何缩放问题有点困难。不过，在转换矩阵的帮助下，[钻 PCB 从未如此简单](http://blog.alessiovaleri.it/using-transform-matrix-for-pcb-drilling-part-1/)。

虽然运行工厂的 Gcode 可能是准确的，但实际制造的 PCB 可能并不准确。如果[阿莱西奥]板上的范围没有与数控铣床的轴线完全对齐，钻孔就会在它们应该在的地方结束。为了解决这个问题，[Alessio]编写了一个 PCB 钻孔转换矩阵计算器。基本思想是通过钻几个孔，[Alessio]能够在一点线性代数的帮助下计算出 Gcode 中所需的任何偏移量。