# 测量不同品牌电池的容量

> 原文：<https://hackaday.com/2012/04/09/measuring-the-capacities-of-different-battery-brands/>

[![](img/29d3a6c92609854cd790ba6deafc9961.png "batteries")](http://hackaday.com/wp-content/uploads/2012/04/batteries.jpg)

作为一个聪明的消费者，在杂货店比较类似产品时，[丹尼斯]通常会看每磅的价格。当需要购买几节 AA 电池时，他没有任何数据。为了解决这个小难题，【丹尼斯】决定[测试几种品牌的电池](http://denishennessy.com/2012/04/08/measuring-battery-capacity-with-an-arduino/)，看看哪一种最划算。

在带回家十几个不同品牌的 AA 电池后，[丹尼斯]打开了 Arduino，开始设计电路。为了测试每个品牌提供的能量，Arduino 每秒测量一个负载上的电压，直到电池达到 0.2V。经过的时间以及电压、瓦特小时、焦耳和环境温度都记录在连接的 LCD 屏幕上，并通过 USB 串行链路发送，以自动执行数据收集过程。

结论是什么？毫不奇怪，像“超级”、“最大”和“超”这样的词并不意味着更好的电池。性价比最高的产品来自一个名为 RS Power Ultra 的非品牌产品。最差的电池是松下 Evolta 电池，每瓦特小时约 1.50 美元。

如果你想验证[Denis]的工作，所有的代码和原理图都在 Github 上。