# 爱迪生试验板适配器的一堆板

> 原文：<https://hackaday.com/2015/04/01/a-stack-of-boards-for-an-edison-breadboard-adapter/>

英特尔 Edison 是一个整洁的硬件，但 Edison 的连接器非常吓人，迷你分线板与试验板不兼容。物联网建设者【费德里科】要做什么？[蚀刻自己的分线板](http://www.instructables.com/id/Plug-your-Intel-Edison-in-a-breadboard/?ALLSTEPS)。

[用于英特尔 Edison 的迷你分线板](https://www.sparkfun.com/products/13025)是官方提供的“最低限度”产品，可以让 Edison 通过大量跳线和 led 启动并运行。虽然这个分线板处理 USB 到 UART 桥、电源调节，并暴露 Edison 连接器上的所有引脚，但它对于原型制作来说很糟糕。这是一个隐藏在爱迪生下面的 0.1 英寸网格上的 4×14 孔阵列。

[费德里科]用覆铜板和一点氯化铁解决了这个问题。他跳进 Eagle，创建了一个分线板，将 4×14 引脚网格变成了一个更合理的试验板友好布局。

支持试验板的适配器没有电平转换器，但通过在 Edison 和试验板适配器之间使用迷你分线板,[Federico]仍然具有 UART 到 USB 硬件和电池充电电路。尽管如此，仍有改进的空间，我们迫不及待地想看看他接下来会想出什么。