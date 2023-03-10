# 给原本只用于仪表的收音机增加公里数

> 原文：<https://hackaday.com/2012/05/18/adding-kilometers-to-a-radio-meant-only-for-meters/>

![](img/b2c4fe717d758b136e90789b83720034.png "high-gain-antenna")

NRF 24L01+无线电收发器可以在许多无线项目中找到。但是它只能在几米的范围内工作。[Achu Wilson]发现他可以将射程大大延长 2 公里。他需要做的就是[建造这个高增益天线](http://blog.achuwilson.in/2012/05/long-range-rf-link-using-nrf24l01-rf.html)。

他已经有了使用射频链路的想法，所以定向天线不成问题。他选择了一个带背反射器的双二阶系统，然后使用 [NEC2](http://en.wikipedia.org/wiki/Numerical_Electromagnetics_Code) 来模拟设计并调整它以获得最佳性能。他只用了大约两个小时就完成了构建，并获得了 10 dB 的增益。对于一些电线和金属薄片来说还不错。

这与 SNES 无线模块中使用的收发器芯片相同。如果我们有一副真正强大的望远镜，我们就可以玩我们一直梦想的超长距离的马里奥赛车游戏了。