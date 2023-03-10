# 使用太阳能电池跟踪太阳为你的太阳能电池(狗)

> 原文：<https://hackaday.com/2012/06/19/using-solar-cells-to-track-the-sun-for-your-solar-cells-dawg/>

![](img/17d1788e63d83b74a5fafc8485ff4227.png "cheap-solar-tracking-hardware")

这个[太阳能电池板使用太阳能电池](http://www.instructables.com/id/2-sun-tracker-circuit)追踪太阳。这是一个非常有趣的技术，而且可以很便宜地实现。

矩形面板正在进行实际的能量收集。下面看到的圆形模块是一些景观灯的太阳能电池。它们被用作传感器，帮助判断该设备是否直接对准太阳。我们已经看到这种类型的事情[是用四个光敏电阻](http://hackaday.com/2012/05/02/sun-powered-stirling-engine-with-automatic-tracking/)完成的。在这种情况下，如果连接了两个景观灯的负极引线，可以从每个面板的正极引线读取电压。如果您测量电压，并使用旋转支架调整位置，直到读数平衡，您可以确保您的阵列获得最佳的阳光量。

[Gtoal]一直试图从这些面板的输出线直接驱动电机，但没有成功。我们确信有一个简单的模拟比较器电路可以实现这一点。抓住一个小的微控制器是另一种选择(一些芯片内置了模拟比较器)。