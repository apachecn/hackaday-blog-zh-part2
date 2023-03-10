# 数字红外热像仪

> 原文：<https://hackaday.com/2012/12/12/digital-ir-theremin/>

[![Digital IR Theremin](img/d08539245b251f7866537e44f62565ea.png)](http://hackaday.com/2012/12/12/digital-ir-theremin/theremin-3/)

这个[数字红外传感器](http://www.pyroelectro.com/projects/digital_ir_theremin/ "Digital IR Theremin")根据物体与其红外传感器的距离产生音调。这里没有微控制器，因为该项目是数字电子课程的[介绍的一部分。相反，它使用一些比较器、晶体管和门，以及一个 555 定时器来制造噪声。](http://www.kickstarter.com/projects/pyroelectro/open-education-an-introduction-to-digital-electron "Open Education: An Introduction To Digital Electronics")

比较器被连接以创建窗口比较器。如果输入介于两个基准电压之间，此配置将输出数字 1，否则输出数字 0。利用这一点，红外范围传感器的模拟输出可以转换为数字值。

555 定时器负责产生输出波形。根据哪个窗口比较器是活动的，特定的电阻器被切换到定时器的 RC 电路中。这允许根据与红外传感器的距离播放不同的声音。

结果是一个方波，其频率取决于物体与红外传感器的距离。通过为每个距离选择正确的阻力，特雷门琴可以调整到特定的音阶。

对于希望学习数字电子学的人来说，这是一个很好的项目，文章在解释理论方面做得很好。休息之后，来看看特雷门琴发出音调的视频。

[https://www.youtube.com/embed/TlXEd6EWcPc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TlXEd6EWcPc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)