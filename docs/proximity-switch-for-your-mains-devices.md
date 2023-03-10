# 电源设备的近接开关

> 原文：<https://hackaday.com/2012/07/08/proximity-switch-for-your-mains-devices/>

![](img/a999111df51612813085e33666046f51.png "proximity-power-switching")

[Ivan 的]朋友制作了一个接近传感器，每当他走开时，它就会关闭 LED 台灯。这个想法非常好，所以[Ivan]决定通过制作这个接近开关插座盒来实现它。

一个锐利的 GP2D12 红外距离传感器是系统的关键。它有一个发射器和接收器，结合起来根据反射回探测器的光量给出距离反馈。这表现为由 ATtiny85(运行 Arduino 引导程序)监控的电压曲线。它足够小，可以与一个小型变压器和线性调节器一起安装在出线盒内，为逻辑电路供电。电源由一个继电器切换，继电器使用一个 NPN 晶体管来保护芯片的 I/O 引脚。

休息之后，请观看视频，了解实际情况。添加一个倒计时器应该很容易，这样你就可以在车间里自由走动了。有了这一点，这是一个奇妙的替代[一些其他的自动关闭技术为您的长凳出口](http://hackaday.com/2012/06/30/under-bench-timed-outlets-wont-let-you-leave-the-iron-on/)。

[https://www.youtube.com/embed/flChhdJ3hzM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/flChhdJ3hzM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)