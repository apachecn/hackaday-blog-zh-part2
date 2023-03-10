# ATTiny85 上的位碰撞以太网

> 原文：<https://hackaday.com/2014/08/29/bit-banging-ethernet-on-an-attiny85/>

[![Ethernet bit banging](img/bd5e32d26b87355c708a3b2a4db873cf.png)](https://hackaday.com/wp-content/uploads/2014/08/ethernetbitbanging.png)

[Cnlohr]刚刚发表了一个巧妙但危险的方法来使用 ATTiny85 发送以太网数据包。ATtiny 直接驱动标准以太网电缆的一对差分 TX 线。这样做将迫使 TX 信号接地与 ATTiny 的相同，在某些情况下，如果您的电缆插入以太网供电交换机，可能会在 AVR 上施加 48V 的电压……这可能是一个问题。

在下面嵌入的视频中，[cnlhor]解释说，微控制器的时钟频率为 20Mhz，可以对曼彻斯特编码的电信号进行位爆炸。使用一个巧妙的技巧，他的家庭交换机将检测到他的平台是一个 10 兆位的以太网交换机，然后可以向他的计算机发送硬编码包。正如你所猜测的，每个数据包在 ATTiny 的闪存中占据相当大的空间:2+千字节。所有使用的代码都可以在[创建者的 GitHub 库](https://github.com/cnlohr/ethertiny)上下载，尽管他不断警告我们不应该将它用于现实生活中的应用。

编辑:我们的一位读者也让我们知道了一个类似的令人敬畏的项目，叫做 [IgorPlug-UDP](http://www.cesko.host.sk/IgorPlugUDP/IgorPlug-UDP%20(AVR)_eng.htm) 。一定要去看看！

[https://www.youtube.com/embed/mwcvElQS-hM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mwcvElQS-hM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)