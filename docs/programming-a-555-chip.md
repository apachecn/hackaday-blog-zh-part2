# 对 555 芯片进行编程

> 原文：<https://hackaday.com/2013/02/08/programming-a-555-chip/>

![555](img/c227e18ac48721f5d9759f0f14986d79.png)

[Phillip]需要一种每 8 小时左右触发一次输入的方法。这是一个带有适当定时器的微控制器的快照，但他最近听说了一个非常酷的可编程定时器芯片，也是 555。当然，CSS555 定时器芯片有一个模糊的编程接口，但这不是一个问题[当你可以用并行端口自己编程](http://www.jameco.com/Jameco/workshop/mystory/CSS55-timer.html)时。

[CSS555 定时器芯片](http://www.customsiliconsolutions.com/downloads/Revised%20Standard%20products/CSS555_App_Note1_Serial_Interface.pdf) (PDF…)是个奇怪的小野兽。它与每个人都喜欢的定时器 IC 引脚兼容，但也有一种编程模式，允许输出每 1 个周期触发一次，每 10 个周期触发一次，以此类推，最高每 100 万个周期触发一次。基本上，它是一个带有巨大可编程电容器[的 555，只需要两块钱](http://www.jameco.com/webapp/wcs/stores/servlet/ProductDisplay?langId=-1&storeId=10001&productId=2146450&catalogId=10001&CID=MERCH)。

在用 74125 十六进制缓冲芯片构建了一个编程电路后，[Philip]将他的编程器连接到一台老式个人电脑的并行端口上。为了一点逆向计算的可信度，他在 Forth 中编写了一个小应用程序，将命令从并行端口推送到 CSS555 芯片，大大增加了芯片股票配置的时间延迟。

这是一个整洁的构建，也是一个非常酷的定时器芯片的精彩介绍。当然，这可以很容易地用 2 美元的微控制器复制，但这不会给[菲利普]使用 555 的满足感。