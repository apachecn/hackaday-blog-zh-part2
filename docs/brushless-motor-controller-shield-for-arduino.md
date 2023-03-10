# Arduino 无刷电机控制器护罩

> 原文：<https://hackaday.com/2014/10/08/brushless-motor-controller-shield-for-arduino/>

无刷电机在 RC 应用和机器人中普遍存在，但通常由低成本电机控制器驱动，这些控制器必须用 RC 式 PWM 信号控制，不允许太多定制。虽然已经有几个开源的无刷驱动器可用，但[neuromancer2701]在 Arduino shield 上创建了自己的[无刷电机控制器。](http://hackaday.io/project/1490-openbldc)

[neuromancer2701]的屏蔽是无传感器设计，这意味着它使用电机的反电动势进行反馈，而不是安装在电机上的霍尔效应传感器。让这些传感器闲置似乎有些奇怪，但这可以让更便宜的无传感器电机配合系统工作。它还使用分立场效应晶体管代替集成驱动集成电路，[类似于我们已经介绍过的](http://hackaday.com/2011/05/24/building-a-brushless-motor-controller/)的其他设计[。尽管他仍在固件中研究反电动势感测，但防护罩成功地以开环模式驱动电机。](http://hackaday.com/2013/10/19/build-a-sensorless-brushless-dc-motor-controller/)

电机控制器通过 Arduino 的串行接口进行控制，未来将支持与 ROS(机器人操作系统)的串行接口。对于需要可定制的开源电机控制器的机器人来说，这种屏蔽可能是 hobby RC 控制器的一个很好的替代选择。GitHub 上有[的 PCB 设计和源代码。](https://github.com/Neuromancer2701/BLDC_ros_controller)

[https://www.youtube.com/embed/lX-jWYU5Xhg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lX-jWYU5Xhg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)