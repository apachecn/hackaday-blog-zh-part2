# 西蒙说学习如何给 ARM 芯片编程

> 原文：<https://hackaday.com/2013/07/05/simon-says-learn-how-to-program-arm-chips/>

![barebones-simon-says](img/17fe48604cec5a2b167b55f9b90f8f34.png)

这个西蒙说游戏的[试验版是在新的微控制器平台上尝试你的技能的好方法。电路板中央的 8 引脚芯片是 LPC810 微控制器，[Hartmut Wendt]刚刚开始使用它。这是 ARM 器件(Cortext M0)采用低引脚数 DIP 封装的罕见例子。试验板友好的外形使其易于使用，但您也可以使用开发板(如 STM discovery 产品或 Stellaris Launchpad 板)实现相同的构建。](http://www.hwhardsoft.de/english/projects/simon-says/)

为什么这是学习的好方法？它包括输入、输出和生成波形，我们假设这些波形是指计时器(我们没有深入研究上面链接的页面中提供的源代码)。每个彩色按钮有一个匹配的发光二极管，闪烁出你必须复制的模式，以保持游戏继续进行；你知道西蒙怎么说的，对吧？。同时，右边的扬声器播放不同的音调。

另一个很好的做法是将[哈特穆特的]代码移植到不同的芯片上，不管是 ARM 还是其他芯片。

[https://www.youtube.com/embed/AJpPCqQdsoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AJpPCqQdsoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)