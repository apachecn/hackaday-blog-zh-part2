# PID 控制胶枪

> 原文：<https://hackaday.com/2014/08/15/pid-controlled-glue-gun/>

[![Internals of a glue gun controlled with a PID controller](img/f73d3be97a1416910c6d1a78e0fa26cc.png)](http://hackaday.com/2014/08/15/pid-controlled-glue-gun/gluegun-pid/)

热熔胶属于管道胶带和拉链带的同一类别，是一种用于固定任何需要粘在一起的东西的通用材料。[Ed]的博世胶枪为他提供了很好的服务，但几年后，温度调节停止工作。他决定把它拆开，而不是买新的。

随着旧的温度调节电路的成熟，[Ed]四处寻找易贝更好的东西。他偶然发现了一个廉价的 PID 温度控制器，于是 [Frankengluegun](http://www.estechnical.co.uk/blog/entry/frankengluegun-making-a-low-cost-temperature-controlled-glue-gun) 诞生了。

使用贴有一些 kapton 胶带和导热膏的热电偶来测量机筒的温度。胶枪的电源通过 PID 控制器传输，PID 控制器使用 PWM 来精确控制温度。所有的电线甚至可以通过原来的线夹进行布线。

有精确温度控制的优质胶枪相当昂贵。这种溶液可以以不到 30 美元的价格添加到胶枪上，最终产品看起来也一样好。