# 惯性导航系统导论

> 原文：<https://hackaday.com/2013/07/31/an-introduction-to-inertial-navigation-systems/>

![acc_sens](img/378b2830ade0a28cf28f382e5368ee1b.png)

早在船只依靠 GPS 来确定位置之前——甚至在罗兰等无线电导航系统出现之前，船只就依靠一种仍然令人印象深刻的复杂手段来确定位置:惯性导航。理论很简单:如果你在船上放几个非常精确的陀螺仪和加速度计，你就能计算出你相对于先前位置的位置。由于电子陀螺仪和加速度计无处不在，[Sebastian]认为他应该尝试创建自己的惯性导航系统。

使用这种方法的困难在于，每个陀螺仪都不可避免地存在一些误差。因为来自陀螺仪和加速度计的测量值被集成在一起，所以误差也被集成，导致定位误差随着时间的推移而增加。通过一些巧妙的算法和非常好的传感器，有可能将这种误差降至最低。

[Sebastian]没有真正好的硬件——他只使用了一个[加速度计/陀螺仪转接板](https://www.sparkfun.com/products/11028),对于实验目的来说已经足够好了。在用 Arduino 读取加速度计数据后，他能够捕获所有传感器数据并将其读入 Python 脚本。

下一步是找出一个体面的算法来整合所有的传感器数据，并可能增加一个气压计和磁罗盘，以更好地补偿误差。该项目仍处于早期阶段，但鉴于惯性导航系统是 20 世纪初的工程胜利之一，我们热切期待任何进展更新。