# 非常非常小的惯性测量单元

> 原文：<https://hackaday.com/2015/05/20/a-very-very-small-imu/>

我们玩四轴飞行器、飞行控制器、运动控制玩具和数百种其他小玩意的原因是 MEMS 革命。微型加速度计和陀螺仪有很多可能，这看起来是迄今为止最小的 IMU。这是一个直径为 18 毫米的 IMU，具有射频网络、C/C++库和 48MHz ARM 微控制器，非常适合我们见过的最小、最强大的四轴飞行器。

这一构建始于对基于 ATMega32u4 的一个非常小的矩形板的扩展。虽然 IMUduino 非常适合通过蓝牙追踪位置和方向，但它仍然只有 4 厘米小。Femtoduino 将它切割成一个 18 毫米的圆形，大小刚好可以塞进模型火箭或飞机。

现在，femtoIO 正在为这些主板的测试版运行一个非常合理的 Kickstarter，目标是 500 美元。电路板本身有点贵，但这就是 9 自由度 IMU 和高度计/温度传感器的价格。