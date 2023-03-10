# MSP430 Launchpad 的逻辑分析仪附件

> 原文：<https://hackaday.com/2012/07/09/logic-analyzer-add-on-for-the-msp430-launchpad/>

![](img/76bf81b0da5080b042bf161e5359e466.png "msp430-launchpad-logic-analyzer-add-on")

这里有一个用于 MSP430 发射台的 6 通道逻辑分析仪屏蔽。它每秒处理令人吃惊的 1600 万个样本。上面看到的原型是用点对点焊接在一块原型板上制作的。[负鼠]确实设计了一个 PCB——只有 50 毫米×50 毫米——但是还没有生产出来。

他称之为 LogicBoost，并将其基于 LogicShrimp 设计。8 引脚芯片的六元组都是 SPI RAM。它们负责存储样本，用 74HC573 锁存器路由流量。MSP430 芯片提供 SPI 时钟，Launchpad 的虚拟 com 端口可用于将数据推送到计算机进行绘图。这有点慢，所以[oPossum]还包括一个可选的 FTDI 板接头，可以更快地完成工作。可以通过调整芯片的内部振荡器设置来调整采样率；有很多选择，所以它几乎可以用于任何目的(只要你不超过 16 Msps 的速度限制)。

[via [危险原型](http://dangerousprototypes.com/2012/07/05/msp430-launchpad-logic-analyzer-based-on-the-logic-shrimp/)