# 构建无传感器无刷 DC 电机控制器

> 原文：<https://hackaday.com/2013/10/19/build-a-sensorless-brushless-dc-motor-controller/>

[Davide Gironi]向我们展示了如何使用 ATmega8 微控制器实现[无传感器无刷 DC 电机控制器](http://davidegironi.blogspot.it/2013/09/a-simple-brushless-sensorless-motor.html)(无传感器 BLDC)。为了控制 BLDC 电机，你需要知道它的旋转顺序位置和速度，这样你就可以计算出正确的电流相序，并在正确的时间应用于电机绕组。

简而言之，无传感器 BLDC 意味着您不使用专门构建的传感器来确定电机的位置和速度，但是，您使用来自当前未通电的电机线圈之一的反电动势信号来检测电机的序列位置。当该反电动势信号越过零电压时，微控制器可以计算转速以及何时切换到下一个电源序列。这种技术不适用于位置控制电机，但适用于连续电机，如计算机风扇和驱动器，略微降低的布线成本使这种类型的 BLDC 控制受到青睐。

如果你想建立一个 BLDC 控制器，我们建议从【大卫的】上一个关于[传感器控制的 BLDC 汽车](http://hackaday.com/2013/09/21/building-a-brushless-motor-controller-around-an-atmega-chip/#comment-1069217)的项目开始。您还可以查看[这些互动演示](http://us.nanotec.com/support/tutorials/stepper-motor-and-bldc-motors-animation/)，以更多了解不同的 BLDC 配置。

休息之后，请继续观看视频演示,[Davide 的]无传感器 BLDC 控制器从光盘驱动器控制电机。

[https://www.youtube.com/embed/bljcl14v8NQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bljcl14v8NQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)