# 超级碗足球灯让你随时了解

> 原文：<https://hackaday.com/2015/02/04/super-bowl-football-lamp-keeps-you-informed/>

[大卫]喜欢看足球。在他喜欢的球队输掉季后赛后，他想找另一个理由去看上周日的大赛。他最终为自己建造了一个足球形状的灯，可以根据谁最后得分而改变颜色。

[大卫]从一个[火花核心](http://hackaday.com/2015/01/02/shower-occupancy-sensor-keeps-peaceeliminates-odor-at-the-office/ "Spark Core Project")和一个火花按钮开始。Spark 是主要的微控制器，包括 WiFi。火花按钮本质上是火花的防护罩，包括一个加速度计、一些发光二极管和几个按钮。这个建筑的另一部分是房屋。[大卫]用他从游行中免费得到的玩具足球。

至于代码，[David]首先从学习如何控制 Spark 按钮上的 led 开始。然后他编写了自己的达阵函数，用特定的颜色照亮足球。由于 Spark 使用 REST API，[David]只需访问他的 Spark 的 URL 就可以触发这个函数。这使得触发事件变得非常简单。

多亏了 [IfThisThenThat](http://hackaday.com/2013/06/01/complicated-iphone-garage-door-opener/ "If This Then That Project") (IFTTT)，这个构建的最后部分变得很容易。这是一个 web 服务，允许您监视各种在线 web 服务并与之交互。它可以监视一个服务，然后根据第一个服务中发生的事件与另一个服务进行交互。在这种情况下，[大卫]使用的是 ESPN 添加到 IFTTT 的“通道”。当您指定的任何团队发生特定事件时，该通道会触发。对于这个项目，[大卫]是监测达阵。

在综合了所有这些不同的服务之后，[大卫]有了一个可以根据哪个队得分而改变颜色的工作灯。他确实注意到 IFTTT 有 1 到 15 分钟的延迟，他希望通过直接挂钩 API 并完全跳过额外的服务来改进这种设计。