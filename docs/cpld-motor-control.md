# CPLD 电机控制

> 原文：<https://hackaday.com/2012/08/02/cpld-motor-control/>

![](img/99b7b6e2d8ee8d5858b2431b7227dc18.png "fpga-motor-controller")

[Chris]继续制作教程，这一次他向[展示如何使用 CPLD 进行简单的电机控制](http://www.pyroelectro.com/tutorials/fpga_motor_control/data.html)。演示硬件非常简单，他[几年前建造了他自己的 FPGA/CPLD 演示板](http://www.pyroelectro.com/tutorials/cpld_board/index.html)，它使用了一个 PLCC 插座以方便接口。你应该可以使用手头上的任何装备。

当然，关于这些芯片的事情是，你正在与可以并行运行的硬件一起工作。[Chris]提到这是它非常适合时间关键型应用的原因。这里，他使用一个电机驱动器来监控 PWM 信号，利用占空比来控制电机转动的方向和速度。休息之后，您可以看到 CPLD 从 ADC 芯片读取数据并将该值转换为 PWM 信号的演示。[Chris]也对 VGA 信号使用了相同的硬件；如果用微控制器来做，这通常是一个定时噩梦。

如果这让你渴望更多的 CPLD 优点，看看我们自己关于这个主题的指南。

[https://www.youtube.com/embed/0zIejq-sRH4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0zIejq-sRH4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)