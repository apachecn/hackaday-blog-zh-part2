# 将铣床改造成数控机床

> 原文：<https://hackaday.com/2013/10/25/converting-a-mill-to-cnc-2/>

[![traces](img/ca054709787ce49ac6429d460384f863.png)](http://hackaday.com/wp-content/uploads/2013/10/traces.jpg)

有一个你想自动化的工厂吗？也许你可以从[詹姆斯]最近完成的工作中得到一些启发。使用熟悉的 NEMA 23 步进电机(RepRap 中使用的相同电机)，他[破解了他的 prox on MF-70 研磨机](http://www.jamesglanville.com/wordpress/converting-a-proxxon-mf-70-mill-to-cnc/)用于 CNC 控制。加上 Sanguino 和其他项目的步进控制器，[詹姆斯]以最小的投资获得了一台工作机器。你可以看出[James]是一个多态迷，因为他在项目的大部分时间里都在大量使用它，甚至用它来创建一些 [Oldham 耦合](http://www.jamesglanville.com/wordpress/making-oldham-couplings/) ( [Google cache](http://webcache.googleusercontent.com/search?q=cache:http://www.jamesglanville.com/wordpress/making-oldham-couplings/) )。

在完成最初的构建后，他试图通过过快地铣削钢材来烧坏主轴电机。我们发现有趣的是，他能够使用 TURNIGY 2217 860kv 22A Outrunner(用于遥控飞机)作为新的主轴电机。它不仅是一个低成本的解决方案，而且与传统的无刷 ESC 配对可以让您的 CNC 软件直接控制电机速度。

上图是一个例子，展示了[詹姆斯]机器的能力。总的来说，对于我们大多数人来说，这是一个非常容易实现的项目。不是每个轧机都需要[有 10 密耳的走线能力](http://hackaday.com/2013/08/16/101459/)。如果你有这个冲动，你可以自己组装一个。当然，如果你有，请告诉我们！