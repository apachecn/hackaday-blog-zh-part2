# 详细了解 7805 电压调节器

> 原文：<https://hackaday.com/2014/09/08/a-detailed-look-at-the-7805-voltage-regulator/>

我们很肯定，所有的爱好者都至少使用过一次 7805 稳压器。它们是将 7V+电压调节至 5V 的简单方法，而这正是我们一些低功耗项目所需要的。[Ken Shirriff]写了一篇[非常详细的文章](http://www.righto.com/2014/09/reverse-engineering-counterfeit-7805.html),介绍其在硅世界中的操作和实现理论。

如上图所示，这种稳压器由不同的元件组成:晶体管、电阻、电容和二极管，它们都集成在芯片中。[Ken]为我们识别它们提供了必要的线索，然后解释了 7805 如何能够在温度变化时保持稳定的输出。这是通过使用[带隙基准](http://en.wikipedia.org/wiki/Bandgap_voltage_reference)来实现的，其中高电流和低电流的晶体管基极-发射极电压之间的差异用于抵消温度的影响。由于在[Ken]的逆向工程过程中有些元素看起来有点奇怪，他最终得出结论，他在 Ebay 上购买的东西可能是假冒的(阅读此 [Reddit 评论](http://www.reddit.com/r/ReverseEngineering/comments/2fn7fd/reverse_engineering_a_counterfeit_7805_voltage/ckb2lk0)以获得另一种意见)。