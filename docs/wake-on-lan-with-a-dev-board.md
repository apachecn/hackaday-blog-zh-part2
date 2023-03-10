# 使用开发板在局域网上唤醒

> 原文：<https://hackaday.com/2014/05/19/wake-on-lan-with-a-dev-board/>

![Screen](img/06d2b833efe6efebdfeea3cdb31afb18.png)

在家里，[Daniel]有一个非常强大的带 ECC RAM 的双四核至强系统，他用它来完成繁重的任务——编译、CUDA 处理和实际的*计算*。当然，一直运行这个盒子的电费会很高，所以就这样吧。只有一个问题:由于某种原因，BIOS 没有局域网唤醒功能。当然，解决方案是一个微控制器系统，它会监听神奇的 WoL 包，并在收到包时打开计算机。[这个项目最终变成了一个很好的案例模块](http://hackingbeaver.com/?p=194)，它带有一个集成的 LCD，可以通过以太网给计算机供电，显示当前运行的进程、CPU 和内存使用情况，是 TI 开发板的一个很好的用途。

问题中的开发板是一个运行 Linux 的 TI Sitara AM355x 入门套件，有两个以太网端口和一个触摸感应 LCD，处理像系统监视器这样简单的事情绰绰有余。为了从开发板启动他的巨型计算机，[Daniel]使用了开发板上的 LED、逆变器、ULN2003 驱动芯片和连接到计算机电源按钮的继电器。这不完全是一个工艺杰作，但开发板安装在机箱中看起来很好，从下面的视频来看，这是一个将系统信息嵌入计算机机箱的好方法。

[https://www.youtube.com/embed/p6rZr09zxkw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/p6rZr09zxkw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/ZVMk-6AnzJI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZVMk-6AnzJI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)