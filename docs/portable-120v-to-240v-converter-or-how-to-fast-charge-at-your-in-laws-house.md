# 便携式 120 伏至 240 伏转换器；或者怎么在亲家快充

> 原文：<https://hackaday.com/2015/03/21/portable-120v-to-240v-converter-or-how-to-fast-charge-at-your-in-laws-house/>

[Nick Sayer]属于“宁可自己造也不买”一类。这个特别的项目是快速电动汽车充电器的克隆。市场上有以 *Quick 220* 品牌出售的版本。这个想法是为了快速充电，一些电动汽车需要 240V 的插座，而没有电动汽车的美国人通常没有。如果有的话，那是为了像炉子或干衣机这样的电器，可能在车库里找不到。

该设备使用两个火线和一个地线来提供 240V 输出，在一些三相电源的业务中，这将接近 208V，但仍应工作。显然，除非你确切知道它是如何工作的，否则你不应该这样做，我们赞扬[Nick]在提供这些担忧背后的知识的同时传播这些危险。

强大的转换器的两个输入不仅由独立电路上的插座提供，而且由热线相位相差 180 度的两个电路提供。这意味着要识别出哪里有两个不受 GFCI 插座或断路器保护的插头，它们位于分相电源的两条单独的热线上。为了保护用户，[Nick]设计了一套继电器，当两个电源中的一个被拔掉时，它就会切断电路。没有这些保护的系统会在断开的插头上有电源电压。

我们很少看到汽车充电黑客。如果你知道一个，或者一直在自己工作，[让我们知道](http://hackaday.com/submit-a-tip/)！