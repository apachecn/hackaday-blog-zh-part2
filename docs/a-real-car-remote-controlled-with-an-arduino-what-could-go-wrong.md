# 一辆用 Arduino 遥控的真车…会出什么问题？

> 原文：<https://hackaday.com/2013/09/01/a-real-car-remote-controlled-with-an-arduino-what-could-go-wrong/>

[![](img/5ba47e3ba927d841650e25aec9109387.png)](http://hackaday.com/wp-content/uploads/2013/09/fd1h4zthkzavjfz-large.jpg)

[吉拉德]向我们透露了他的最新项目，他在妻子的汽车中添加了大量的气动和电子设备，以遥控汽车。

刹车/油门踏板由电子阀控制的活塞驱动，一个标准的 DC 发动机负责转动车轮。Arduino 代码告诉我们，只要远程上/下通道高于/低于给定值，阀门就会打开。框架基于 Festo 铝型材，我们不确定用于 DC/DC 转换器的电源来自哪里。由于阀门使用 24V，电机使用 12V，标准 N-MOSFET 和功率继电器用于电压转换。[吉拉德]使用的遥控器实际上已经有 20 年的历史了，所以接收器的输出信号实际上并不干净。

我们真的希望永远不要在路上看到这辆车…