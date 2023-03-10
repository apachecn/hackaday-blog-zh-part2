# 使用 SDR 读取您的智能电表

> 原文：<https://hackaday.com/2014/02/25/using-sdr-to-read-your-smart-meter/>

[BeMasher]对读取他的智能电表的其他解决方案的成本不满意，所以[他做了一个项目，使用 rtl-sdr 加密狗](https://github.com/bemasher/rtlamr)自己读取电表。

利用他的黑客和逆向工程技能以及一个 20 美元的 RTL-SDR 加密狗，[BeMasher]编写了 [rtlamr 来自动检测和报告](http://bemasher.github.io/rtlamr/)范围内智能电表报告的消耗信息。虽然是为他的 Itron C1SR 设计的，但[BeMasher]声称任何支持电子收发机(ERT)的智能电表都应该可以工作。

[BeMasher]的 Itron C1SR 智能电表使用曼彻斯特编码的跳频扩频协议，在 915MHz ISM 频段广播间隔数据和标准消耗。[BeMasher]使用 RTL-SDR 加密狗进行信号捕获，然后在软件中分析产生的信号。[BeMasher]很好地完成了分析最终数据捕获的理论和实现[,因此一定要检查它以进行深入分析。](http://bemasher.github.io/rtlamr/2014/02/08/innards.html)

如果 RTL-SDR 加密狗对你来说太有限了，你可能想[看看一些黑客友好的 SDR，有一点更强的冲击力](http://hackaday.com/2013/08/23/a-comparison-of-hacker-friendly-sdrs/)。