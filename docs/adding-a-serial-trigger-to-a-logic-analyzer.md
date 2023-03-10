# 向逻辑分析仪添加串行触发器

> 原文：<https://hackaday.com/2012/08/08/adding-a-serial-trigger-to-a-logic-analyzer/>

![](img/5f5e461e96db9f4f30a7bb0697eaa166.png "logic")

如果你试图用一个简单的逻辑分析仪调试一个串行总线，你会有一段不好的时间。大多数廉价的分析器都没有串行模式触发器，也没有在特定的位模式进入管道后开始记录数据的方法。[Neil]提交了一个很棒的小项目，[为这些分析器](https://sites.google.com/site/eecsprojects/home/digital-system-projects/adding-serial-pattern-trigger-feature-to-logicport)添加了一个串行触发器，我们不得不称赞他设计了如此有用的电路板。

[Neil]设计了一个小型电路板，具有 CLPD，可将串行数据转换为并行数据。通过将逻辑分析仪的触发条件设置为他想要的任何 24 位模式,[Neil]可以在他想要的时候准确地嗅探串行总线。

该电路非常简单，基本上只有一个 100 引脚的 CLPD 和一堆 0.100”的接头引脚。这是一个有用的工具，尽管我们找不到董事会文件来制作我们自己的，但我们确信[Neil]将很快提供它。