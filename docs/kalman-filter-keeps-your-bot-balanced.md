# 卡尔曼滤波器让你的机器人保持平衡

> 原文：<https://hackaday.com/2012/09/10/kalman-filter-keeps-your-bot-balanced/>

![](img/7515971cca09bf1ca023754d4666b032.png "kalman-filter")

如果你想提高你的自平衡机器人的稳定性，你可能会使用一个简单的可怕的等式，就像这个一样。当[为他的平衡机器人](http://blog.tkjelectronics.dk/2012/09/a-practical-approach-to-kalman-filter-and-how-to-implement-it/)开发传感器过滤算法时，这是【劳斯苏斯】旅程的一部分。他没有突破新的数学思想，但试图让下一个人更容易使用[卡尔曼滤波器](http://en.wikipedia.org/wiki/Kalman_filter)。这是一种抑制噪声和平均机器人应用中常用的传感器数据的方法。

他的机器人使用陀螺仪和加速度计，只用两个轮子就能保持直立。这些传感器的组合提出了一个有趣的问题，即加速度计输入在较长时间内采样时最为精确，而陀螺仪则相反。该滤波器考虑了这些特性，同时也排除了传感器噪声。尽管上面的图表令人望而生畏，但[Lauszus]在分解更大的函数并向我们展示从哪里获取数据以及如何在微控制器代码中使用数据方面做得相当出色。