# 视觉障碍者用声学导航仪

> 原文：<https://hackaday.com/2013/12/31/acoustic-wayfinder-for-the-visually-impaired/>

![](img/90e7276090909d12814da38d1fe153bc.png)

理想情况下，技术应该改善我们的生活。康奈尔大学的两位高年级学生[Shane 和 Eileen]发现了一种很好的方法，用他们的声学寻路设备来改善视障人士的生活。在为他们的最终项目进行头脑风暴时，[谢恩和艾琳]受到了[这篇关于机器人作为导盲犬可行替代品的黑客帖子的启发。他们试图提供可佩戴的免提导航和(主要)室内障碍物检测——即椅子、长凳和其他低于眼睛高度的无生命物体。](http://hackaday.com/2012/09/05/can-a-robot-be-a-safe-and-cost-effective-alternative-to-guide-dogs/)

该探路者包括两个协同工作的系统:一个头戴式导航单元和一个戴在用户手指上的触觉传感器。这两个系统都使用 [Maxbotix LV-MaxSonar-EZ0](http://www.maxbotix.com/Ultrasonic_Sensors/MB1000.htm) 超声波测距仪模块来检测障碍物，并使用[振动微型圆盘电机](http://www.adafruit.com/products/1201)以与用户离障碍物的距离成比例的速度提供触觉反馈。

主机使用两个测距仪和两个振动马达。这些测距仪的视野约为 120 度，能够探测到 6.45 米以外的障碍物。触觉传感器由一个测距仪和电机组成，使用方式类似于[吸尘器手杖](http://en.wikipedia.org/wiki/White_cane)。用户挥动他们的手来检测可能在主机范围之外的物体。这两个部分都符合人体工程学，尺寸可调。

开机时，[Shane 和 Eileen]的软件会对触觉传感器进行校准，以结合用户的身高确定距离阈值。他们使用 ATMega 1284 来驱动系统，并使用 [TinyRealTime 内核](http://www.control.lth.se/~anton/tinyrealtime/)处理两个子系统之间的实时任务调度。休息之后会嵌入完整的演示视频。

 [https://www.youtube.com/embed/uGR3G30FyMc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uGR3G30FyMc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢谢恩和艾琳]