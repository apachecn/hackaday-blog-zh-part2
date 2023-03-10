# 如何:侵入自己的封闭社区

> 原文：<https://hackaday.com/2014/07/14/how-to-hack-your-way-into-your-own-gated-community/>

![RF Signal Decryption and Emulation](img/f5db2f0e32bab9a2ba6b63779a1970d4.png)

你的门控社区让你感到安全，因为远程控制的大门阻止了痞子吗？自从[Tomasz]模仿打开入口大门的信号入侵了他自己的社区以来，波兰这种封闭式社区的居民现在都在恐惧中颤抖。令人震惊的是，这从开始到结束只花了大约 4 个小时，部分只花了大约 20 美元。

大多数这类系统都使用射频通信，托马斯的也不例外。第一步是记录他的遥控器发出的信号。一个 [USB 软件定义的无线电发射器/接收器](http://www.rtl-sdr.com/about-rtl-sdr/)与一个名为 [SDR#](http://sdrsharp.com/) 的程序耦合，顺利读取并记录信号。[Tomasz]期待着一个连续的通信，但在记录和分析了几个进入社区的人的信号后，很明显每个人的遥控器都只有一个代码。

现在他知道了密码，[托马斯]必须想办法把信号发送给接收者。他用少量的零件制造了一个射频发射器，肉和土豆是一个科尔皮兹振荡器和一个功率放大器。这个简单的发射器连接到负责调制任务的[发现](http://www.st.com/web/en/catalog/mmc/FM141/SC1169/SS1295?sc=stm32l1)板。[Tomasz]很好，他把自己的代码放在自己的网站上，供任何有兴趣的人访问。