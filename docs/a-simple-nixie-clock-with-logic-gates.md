# 一个简单的带逻辑门的谢妮时钟

> 原文：<https://hackaday.com/2013/09/27/a-simple-nixie-clock-with-logic-gates/>

[![](img/9bd184587dd6640f105332a4f0fc53e6.png)](http://hackaday.com/wp-content/uploads/2013/09/fypvvro.jpg)

这里有一个[Znaxque]几个月前完成的非常好的项目:一个只用逻辑门制作的简单的谢妮时钟。在这个版本中，电源 50Hz 被用作时基，而不是这里大多数读者可能使用的 32KHz 晶体。从*非常*长远来看，这个时钟实际上可能比基于晶体的时钟更精确，因为欧洲的电力公司调整电源频率。然而，在给定的时刻，这个时钟和一个参考之间的差异可能会大到 [60 秒](http://wwwhome.cs.utwente.nl/~ptdeboer/misc/mains.html)。

这个设计是在一张简单的纸上画的草图，后来用回收的集成电路制作而成。[Znaxque]只花了 45 美元买了 6 个 IN-14 nixies 和上图所示的 veroboard。BCD 至十进制解码器为 74141，板上有三个按钮用于设置分钟、小时以及重置所有计数器。