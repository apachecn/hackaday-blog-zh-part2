# 室内直升机的通信协议

> 原文：<https://hackaday.com/2013/01/21/communication-protocol-for-an-indoor-helicopter/>

![propel-execuheli-ir-protocol-revealed](img/ca5fe851b6720575bf40c28b6584b2ea.png)

有一种特殊的满足感来自于在逆向工程项目结束时真正理解一些东西是如何工作的。上面这个网格是[斯潘塞]努力逆向工程一个 Propel ExecuHeli 室内直升机玩具的红外协议的顶点。

他首先看到的是三个不同的控制器通道，可以选择这些通道来允许多架直升机在同一区域使用。[斯潘塞]很惊讶他们都使用相同的载波频率。秘密一定在编码包中，所以他的下一个挑战是弄清楚数据是如何通过红外信号传输的。原来这些包使用的是脉冲长度编码(我们不熟悉这个协议，但是[你可以在这里读到更多关于它的信息](http://irq5.wordpress.com/2012/07/27/infrared-remote-control-protocols-part-1/))。拼图的最后一块是捕获控制模块的每次独特变化所产生的数据包。随着每个位(除了位 11)被考虑，他现在可以为控制器替换格式化他自己的代码。或许他正期待[让直升机自主飞行](http://hackaday.com/2012/03/23/decoding-then-cloning-an-ir-helicopter-toys-control-signals/)？