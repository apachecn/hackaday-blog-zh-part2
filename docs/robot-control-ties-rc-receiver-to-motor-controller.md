# 机器人控制将 RC 接收器连接到电机控制器

> 原文：<https://hackaday.com/2015/07/21/robot-control-ties-rc-receiver-to-motor-controller/>

[Andrey Nechypurenko]发布了他的机器人地面车辆设计指南的第二部分。在他的[第一篇文章](http://hackaday.com/2015/07/01/detailed-robotics-ground-vehicle-design-guide/)中【Andrey】详细描述了他所面临的机械设计决策。[Andrey]现在开始覆盖电气组件，从使用标准无线电控制系统的手动控制开始。为了实现这一点，RC 系统使用了一个 [MD22 h 桥驱动器](http://www.robot-electronics.co.uk/htm/md22tech.htm)和一个 [picoUPS](http://www.mini-box.com/picoUPS-120-12V-DC-micro-UPS-battery-backup?sc=8&category=980) 。

MD22 是一个简洁的电机控制板，可以从无线电控制器接收 PWM 信号，并使用它来驱动 DC 电机。它也可以选择使用 I2C 接口，为与微控制器集成提供了一个很好的迁移路径。在那之前，这不能真正被称为机器人——它更像是一辆遥控车辆。但是他使用的迭代设计和构建过程是一个很好的过程！

picoUPS 提供车载电池充电。由于其 UPS 的传统，它还允许车辆由外部电源供电，这在开发过程中已被证明是有用的。最后，需要一个 5v 调节器来为板载数字逻辑供电。[Andrey]想要一个快速下降的解决方案，预算足够大，以允许未来的扩展，于是选择了 [Pololu D15V35F5S3](https://www.pololu.com/product/2110) ，它可以在一个小巧易用的模块中提供 3.5 安培的电流。

在对系统进行试验后，[Andrey]制作了一个 PCB 来集成所有组件。下一步是在平台上添加传感器和嵌入式计算机。

[https://www.youtube.com/embed/W47cyLSvp90?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/W47cyLSvp90?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)