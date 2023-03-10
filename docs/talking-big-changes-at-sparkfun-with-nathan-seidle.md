# 在 SparkFun 与 Nathan Seidle 谈论重大变化

> 原文：<https://hackaday.com/2015/06/25/talking-big-changes-at-sparkfun-with-nathan-seidle/>

SparkFun，你了解他们，你爱他们。他们把自己列为“在线零售店”，但我记得他们是因为设计良好的分线板、免费日、关于构建电子产品的视频和自动驾驶汽车竞赛。本周，SparkFun 因一个不同的原因让我惊讶，它宣布创始人兼首席执行官[将离职](https://www.sparkfun.com/news/1853)。他不会离开，而是回到工程部门，由别人接管。我昨天和他讨论了这对他、对公司的意义，以及 SparkFun 对未来的规划。

### 不辞而别

[Nate]在 2003 年创建了 Sparkfun，当时他还在科罗拉多大学博尔德分校攻读电子工程学位。他说，想回到他的工程根源是他改变头衔的原因，这至少在 9 或 10 个月内不会发生。不离开公司就离开 CEO 位置的概念在我脑海中引发了很多疑问。

作为创始人，[内特]是董事会主席，并将保留聘用和解雇首席执行官的权力。正如他所说，这在很多公司都很常见。但我相信，董事长每天以不同的角色走进办公室是很少见的。他和他尚未找到的替代者之间的权力动态并不是唯一的棘手问题。SparkFun 已经有一个工程总监，[ [皮特·多克特](https://www.sparkfun.com/users/19939) ]，根据皮特 系列，你可能从他的 *[中知道他。[Nate]在公开发布之前就让员工做好了准备，包括与[Pete]讨论和规划两人如何与工程团队合作。很明显，我们的想法是发展公司，这意味着越来越多的工程工作要做。](https://www.sparkfun.com/news/tags/according-to-pete)*

新任首席执行官将是公司文化的引导者和捍卫者。SparkFun 并不是在寻找“Nate 第二部分”,无论谁被任命为掌舵人，都将有自由做出更好的改变。如果那个人能处理好上述问题，我认为实际上有[Nate]时不时地提供建议将有助于确保公司的创新价值观和精神不会被冲走。

这就是了，一份诱人的工作。有人对组建应用程序感兴趣吗？

## CM 和 EDA

![makey-cm-by-sparkfun](img/96c026ee7d8470dffa901d84e4b1edc0.png)

MaKey MaKey

当我和他进行视频通话时，我想我应该看看公司的其他情况。具体来说，我一直想知道与 SparkFun 的合同制造。我想到了几个值得注意的硬件，SparkFun 在其中充当了 CM 的角色:Makey Makey T1 和 T2 微视 T3。但你也应该知道，他们开发并生产了几种类型的 Arduino 板，包括 Pro、Pro Mini、Fio 和 Lilypad，产量超过 1000 片。这没什么可轻视的，那么 CM 在 SparkFun 是怎么回事呢？

原来[是那个](https://learn.sparkfun.com/tutorials/how-to-sell-your-widget-on-sparkfun)的向导。要点是，SparkFun 希望销售你的产品，并将充当分销商，或制造商和销售渠道。后者是 Makey Makey 的工作方式。该公司既生产又销售这种能把任何东西变成电脑键盘的设备，并向创造者杰伊·西尔弗(Jay Silver)和埃里克·罗森鲍姆(Eric Rosenbaum)支付版税。[Nate]承认他们过去没有非常关注 CM，但现在正在努力增加更多功能。

![2-years of commits to SparkFun's Eagle libraries](img/638dd91bfded08dedf2781ee303efd15.png)

2-years of commits to SparkFun’s Eagle libraries

在开发方面，SparkFun 因其 Eagle 库而闻名，这些库既广泛又维护良好。我想知道随着时间的推移，这是否会变得更加困难，但是维护和发展它只是工作流程的一部分。它所做的是锁定公司使用 CadSoft Eagle 的电子设计自动化软件。但这并不是不可思议的。

该公司实际上开始使用 Protel(后来成为 Altium Designer ),直到许可费变得非常昂贵，超出了他们所需的座位数量。这促使人们转向 Eagle，Eagle 的好处是许可费更低，SparkFun 的客户可以获得零成本(但尺寸有限)的版本。

具有讽刺意味的是，Altium 一直在大力讨好 SparkFun，让他们开始与名为 [CircuitMaker](http://www.circuitmaker.com/) 的新 EDA 产品合作。Altium 的这种新商业模式提供免费使用，只要设计在线存储并公开发布。如果你付费订阅，可以私下保存你所有的设计。

SparkFun 计划尝试一下 CircuitMaker，并将在几个即将到来的项目中与 KiCAD(免费开源 EDA 套件)一起这么做。我们完全同意[Nate]的观点，即需要一个坚如磐石的转换工具，可以在三个软件之间转换零件库。