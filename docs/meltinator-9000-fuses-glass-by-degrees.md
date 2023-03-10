# 熔化器 9000 逐渐熔化玻璃

> 原文：<https://hackaday.com/2014/02/21/meltinator-9000-fuses-glass-by-degrees/>

![kiln](img/6760ed14909330e83803e31aa1be3848.png) 【理查德】的妻子得到了一个 Evenheat 玻璃熔窑，但是 20 岁的温控器坏了。他本可以简单地订购一个替换控制器，但这种解决问题的方法并不能让你一天都不工作。他的妻子想要更多的控制窑，他说服她，建立自己的路要走。于是，[Meltinator 9000 诞生了](http://oprahsfavoritedeathmetal.blogspot.com/2014/02/in-other-news.html)。

【Richard】的设计使用 Arduino Uno 和 Adafruit 显示屏、protoshield 和热电偶读数板。他用一个电阻、BJT 和一个二极管构建了一个简单的继电器驱动器，并将其连接到 13 号引脚及其内置的指示器。让[理查德]高兴的是，所有这些都符合原来的外壳。

[Richard]的软件提供了 25 个融合计划，每个计划有 10 个步骤。每一步都有一个目标温度、温度 变化的速率，以及一个可以随时增加的保持时间。他运行了一个测试程序，以 2550 华氏度/小时的速度将窑炉加热到 1500 华氏度。然后他以 1000 华氏度/小时的速度将其冷却到 500 华氏度，这比他想象的要长。好消息是窑的隔热性很好！【理查德】的 GitHub 上有 [可用的软件。](https://github.com/thecowgoesmoo/MELTINATOR-9000)

没有玻璃窑？喜欢控制啤酒相关的温度？你总是可以以自制的名义黑掉你的炉子。