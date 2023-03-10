# 自平衡机器人会摇晃，但不会倒下

> 原文：<https://hackaday.com/2014/01/09/self-balancing-robots-wobble-but-they-dont-fall-down/>

![](img/e57b72c04533eb1481698074cad5817b.png)[Trandi]可以在他的任务清单上勾选“建造一个自平衡机器人”。过了几个周末，[他造出了这个机器人，用他自己的话来说，设法不过度设计它](http://trandi.wordpress.com/2014/01/05/self-balancing-robot/)。它甚至让他 2 岁的儿子的注意力保持了几分钟，这总是一个优点。

他原本打算重新利用他儿子的一辆遥控车，但不想冒险弄坏它。相反，他设计了一个三角形的 3d 打印底盘来容纳电机和一些齿轮，以适应电机轴和一些重复使用的 Meccano 车轮。[Trandi]的设计采用了一个 [MPU 6050 6-DOF IMU](http://www.robotshop.com/en/6-dof-gyro-accelerometer-imu-mpu6050.html) 来实现平衡动作，并且是基于 Arduino Nano 克隆体构建的。

[Trandi]正在用一个 [L293D](http://www.me.umn.edu/courses/me2011/arduino/technotes/dcmotors/L293/L293.html) 控制电机，它有内置的反激二极管来最小化尖峰。他发现 Nano 克隆体不够强大，无法处理所有事情，所以他添加了一个 L7805CV 稳压器。休息之后，观看[Trandi]可爱的机器人工具在各种类型的地形上行走，有无有效载荷。

身边没有 IMU？你真的不需要一个来建造一个自我平衡的机器人，因为[这个基于红外的小人机器人将展示](http://hackaday.com/2013/09/26/self-balancing-arduino-does-it-without-an-imu/)。

 [https://www.youtube.com/embed/DtnFCy6076o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DtnFCy6076o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [危险原型](http://dangerousprototypes.com/2014/01/06/self-balancing-robot/)