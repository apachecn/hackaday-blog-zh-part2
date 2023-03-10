# 机器人操作系统(ROS) 101

> 原文：<https://hackaday.com/2014/01/29/the-robot-operating-system-ros-101/>

听说过机器人操作系统吗？这是一个 BSD 许可的开源系统，用于从各种硬件控制机器人。这些年来，我们分享了很多运行 ROS 的项目，但是没有关于如何实际使用 ROS 的内容。幸运的是，一家名为 Clearpath Robotics 的机器人公司——他们使用 ROS 做任何事情——已经决定优雅地分享一些关于如何开始使用 ROS 101 的提示和技巧:[机器人操作系统介绍。](http://www.clearpathrobotics.com/blog/how-to-guide-ros-101/)

ROS 系统的美妙之处在于它由一系列独立的节点组成，这些节点使用发布/订阅消息模型相互通信。这意味着硬件无关紧要。你可以使用不同的计算机，甚至不同的架构。[伊利亚·巴拉诺夫]给出的例子是使用 Arduino 来发布消息，使用笔记本电脑订阅消息，甚至使用 Android 手机来驱动马达——这就是灵活性！

看起来他们会做这 101 个帖子的整个系列，所以看看吧——他们已经发布了 numéro 2， [ROS 101:一个实际的例子。](http://www.clearpathrobotics.com/blog/ros-101-practical-examples/)它甚至包括一个准备就绪的 Ubuntu 光盘映像，预先安装了 ROS，可以在 VMWare Player 上使用！

为了激发你使用 ROS 的灵感，来看看这个使用它的 [Android 控制的机器人](http://hackaday.com/2012/08/04/android-controlled-robot-extravaganza/)！或者一个可笑的[轮椅变成的令人毛骨悚然的面部追踪机器人怎么样？](http://hackaday.com/2012/08/14/toorcamp-mc-hawking-robotic-wheelchair/)