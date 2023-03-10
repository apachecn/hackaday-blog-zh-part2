# DIY ARM 原型板

> 原文：<https://hackaday.com/2012/09/06/diy-arm-prototyping-board/>

![](img/fcc8d9add30e0e2fa125e96917e3c25d.png "diy-arm-prototyping-board")

我们对[Danjovic]展示的 ARM 原型板印象深刻。他证明了在封装日益缩小的今天，用 protoboard 和烙铁制作自己的开发工具仍然是可能的。

实话告诉你，如果他设计并蚀刻了他自己的板子，我们可能不会推荐它。但是他不需要[在布局、蚀刻和回流](http://hackaday.com/2011/08/03/an-arm-dev-board-you-can-make-at-home/)上花费时间。相反，它只是一些漆包线和大量的耐心。耐心是因为恩智浦 ARM Cortex-M0 芯片采用 HVQFN 封装。我们不完全确定高压部分([封装字母](http://hackaday.com/2012/08/31/hackaday-links-august-31-2012/)在这一点上不完全清楚)，但 QFN 意味着四方扁平无引线。这意味着芯片上没有脚。所以[Danjovic]把它倒过来粘上，然后点对点焊接，断开所有的针脚。

该板的顶部有一个引导按钮，复位按钮，电源调节，和一个晶体振荡器。他没有提到他用的是什么引导程序，但是一根诺基亚的 USB 线给他提供了将程序加载到芯片上的连接。