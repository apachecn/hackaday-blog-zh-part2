# 基于 AVR Atmega 的 PID 磁悬浮器

> 原文：<https://hackaday.com/2013/12/05/avr-atmega-based-pid-magnetic-levitator/>

[Davide]看到了我们最近关于磁悬浮的帖子，并很快发送了他自己的项目，其中对其工作原理有很好的解释——他还包括了代码，让您自己试试！

他的装置使用 Atmega8 微控制器，该控制器使用脉宽调制(PWM)控制一个 12V 50N 的小线圈。安装在线圈内部的霍尔效应传感器(Allegro A1302)检测到磁体的距离，PID 控制器使用该数据来自动调整线圈的 PWM，以保持磁体就位。Atmega8 以 8Mhz 运行，霍尔效应传感器每 1ms 轮询一次，为 PWM 提供更新值。他还被扔进了一个 RGB LED，当一个物体悬浮起来时，它就会发光！

那为什么会有一个拿着漂浮气球的孩子？[Davide]实际上为他的朋友[Paolo]建造了一个装置，在一个名为 InverART 2013 的艺术博览会上展示！

休息之后，请查看电路图和该器件运行的简短演示视频！

哦，对了，那些对磁悬浮不感兴趣的人可能会喜欢[声悬浮](http://hackaday.com/2013/09/20/diy-ultrasonic-acoustic-levitation/)。

[![magnetic_levitator_atmega_schematics](img/d723cfbe7071745020de3c7669ba6ec7.png)](http://hackaday.com/wp-content/uploads/2013/12/magnetic_levitator_atmega_schematics.png)

(点击查看全尺寸图表)

[https://www.youtube.com/embed/JzccJaQEEYc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JzccJaQEEYc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)