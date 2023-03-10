# 偷车，用收音机按门铃

> 原文：<https://hackaday.com/2013/03/14/stealing-cars-and-ringing-doorbells-with-radio/>

可以用 USB 电视调谐器构建的廉价软件定义的无线电平台最近在 Hackaday tip line 上并没有得到太多的喜爱。谢天谢地，[Adam]发来了一个很棒的指南，介绍如何[完全开放地破解亚 GHz 无线协议](http://adamsblog.aperturelabs.com/2013/03/you-can-ring-my-bell-adventures-in-sub.html)，并在此过程中按门铃、打开汽车，甚至可能放火焚烧房屋。

第一个无线黑客(Adam)设法解决了无线门铃发射器如何与接收器通信的问题。[Adam]连接了一个 [FUNcube 软件定义的无线电加密狗](http://www.funcubedongle.com/)(尽管我们见过的许多 USB 电视调谐器加密狗中的任何一个也可以工作)，并使用 GNU Radio 将接收到的无线电信号发送到一个 WAV 文件。当在 Audacity 中查看这个音频文件时，[Adam]看到了数字数据的泄露信号，留下了一串 1 和 0，这将触发他的无线门铃。

然而，FUNcube 加密狗没有发射能力，因此[Adam]需要一种功能更强的软件定义无线电来模拟门铃发射器的内部工作原理。他在 USRP Ettus Research 找到了一个，这是一个软件设计的无线电，它很好地保持了[巴林特]，[Hackaday SDR extra ordinaire](http://hackaday.com/2012/04/16/playing-air-traffic-controller-with-software-defined-radio/)的忙碌。通过将[亚当]用 FUNcube 加密狗解码的数据发送到 USRP，他只用了几百美元的无线电设备和巧妙的软件就能触发他的无线门铃。

门铃是一个低风险的游戏，所以[Adam]决定加快步伐，通过捕捉和重放遥控器的信号来解锁他儿子的车。现代汽车的无钥匙进入使用滚动码，所以整个努力只是一个派对把戏。其他支持射频的设备，如遥控电源插座，对家庭和办公室的安全是一个更大的威胁，但仍有一个[亚当]设法破解大开。