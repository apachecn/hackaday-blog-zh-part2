# 光盘 POV 时钟

> 原文：<https://hackaday.com/2013/09/28/cd-rom-pov-clock/>

![clock](img/189e4cc60ed081b3773f3c7c1f8e5ac7.png)

[凯尔]想尝试一些新的东西。使用光盘驱动器的[持续视觉时钟。](http://www.wengenroth.co/projects/cd-persistence-of-vision-clock/)

我们已经报道了许多使用硬盘驱动器的 POV 时钟，但是我们认为这是第一次使用 CD-ROM 驱动器。[Kyle]指出，光盘驱动器通常比硬盘驱动器安静得多，这是他选择光盘驱动器路线的主要原因。

这个项目的核心是一个很好的老式 ATMEGA168 和一个用于照明的 RGB LED 灯条。为了测量和保持时钟的转速，凯尔使用了一个红外光电二极管来检测光盘上的参考标记。一个经典的 POV 时钟优雅的建立，一个新的转折！

这个项目很酷的一点是，他实际上并没有像你想象的那样使用光盘驱动器——他扔掉了主轴电机，而是使用托盘弹出电机来旋转磁盘！他这样做是为了直接通过微控制器的 PWM 来控制电机，而主轴电机则需要一个 IC 和一个具有特定电压幅度的可变控制信号。

他还尝试了不同的背景和背景照明，你可以在休息后的视频中看到！

[https://www.youtube.com/embed/u7rVB-Door8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u7rVB-Door8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)