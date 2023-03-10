# 模拟土壤湿度报警器

> 原文：<https://hackaday.com/2012/06/22/analog-soil-moisture-alarm/>

我们看到的大部分土壤湿度监测器都是微控制器的附件。所以我们很高兴[Miceuz]向我们透露了他用模拟部件制造的这个[土壤湿度报警器。在模拟世界中采用这个概念并构建它真的不难。那是因为你只是在测量一个电阻值。但对于我们这些从未真正接触过模拟器件的人来说，这是一个很好的学习项目。](http://wemakethings.net/2012/06/21/plant_watering_alarm/)

高效率运算放大器是这项工作的主要部分。当土壤潮湿时，与单独的电阻分压器提供的参考电压相比，电阻相当低。但是当植物变得干渴，土壤变干时，电阻增加，触发运算放大器点亮 LED，并在蜂鸣器上产生一些噪声(我们对蜂鸣器的工作原理有点困惑)。

不幸的是，这不是一个可行的长期解决方案，因为电池计算显示它只能持续大约四个月。这就是基于微控制器的电路真正的亮点，因为它可以将自己置于低功耗睡眠状态，偶尔醒来读取读数。