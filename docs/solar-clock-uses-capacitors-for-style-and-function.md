# 太阳能时钟在风格和功能上使用电容器

> 原文：<https://hackaday.com/2013/02/19/solar-clock-uses-capacitors-for-style-and-function/>

![solar-clock-uses-storage-capacitors-and-batteries](img/d050ffb4404cb5dfe827fcc6d15e352c.png)

这个太阳能钟是用许多回收的零件建造的。我们发现[Nereus]将[一圈储能电容器和一个电池](http://www.elektroda.pl/rtvforum/topic2502855.html)([翻译为](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&eotf=1&u=http%3A%2F%2Fwww.elektroda.pl%2Frtvforum%2Ftopic2502855.html))结合起来，创造了一种混合储能装置，这很有趣。

机器翻译使得理解这是如何工作的有点粗糙，但是原理图帮助很大。这对太阳能电池来自一些廉价的太阳能手机充电器，为环绕钟面的电容器组供电。如果放在一个阳光充足的房间里，电池将充满电容器，然后馈入 ICL7663 调节器。我们希望听到关于这款器件选择的意见，因为根据我们的经验，线性调节器效率相当低。但无论如何，调节后的能量供给能量电池和时钟马达。当调节器的输出下降时，电池会自动恢复。该项目还包括一个电压表和温度计，它们可以显示在大约六点钟刻度的微型液晶显示屏上。

现在，如果你想要一个完全不用电池的东西，你必须看看[【杰克·巴芬顿的】带太阳能时钟](http://hackaday.com/2011/12/19/jacks-solar-powered-clock/)。

[谢谢马内基宁]