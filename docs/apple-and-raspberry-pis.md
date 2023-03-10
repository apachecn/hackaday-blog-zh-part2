# 苹果和树莓馅饼

> 原文：<https://hackaday.com/2013/12/26/apple-and-raspberry-pis/>

![A2Pi](img/763c59403af9eec72e4df06ba8f466cf.png)

在互联网的深处，有一些疯狂的人对下一代 Apple II 应该是什么样子有一个愿望清单。这台 80 年代逆向计算的梦想机器的能力通常被认为是具有 32 位 CPU、UNIX 操作系统、现代图形和网络的东西。这听起来很像树莓派，所以[Dave] [做了一个 Apple II 到树莓派的适配卡](http://schmenk.is-a-geek.com/wordpress/?p=167)。

让一个 Pi 通过串行连接与一台 Apple II 对话，并不能真正让任何一台机器拥有另一台机器的全部能力。为了解决这个问题，[Dave] [写了两个软件](http://schmenk.is-a-geek.com/wordpress/?p=135)。第一个是 UNIX 守护进程，它监听串行端口连接上的 Apple II，处理 Apple II 键盘连接。第二个软件是在 Apple II 上运行的 ProDOS 磁盘镜像文件。有了这两个软件，[Dave]可以在 Raspi 上运行 Apple，或者在 Apple 上运行 Raspi，来回发送文件和数据没有问题。

除了提供一个奇怪而令人敬畏的 Apple II 到 UNIX 的界面，Apple II Pi 还有很多可能不太明显的优点。[一个 Apple II 紧凑型闪存适配器](http://dreher.net/?s=projects/CFforAppleII&c=projects/CFforAppleII/main.php)可以用作这些经典苹果硬件的内置硬盘，用于 AII 的 [Uthernet 以太网卡带来了网络。与 Apple II Pi 的组件成本相比，这两种设备都贵得离谱，它们带来的东西很容易被 Apple II Pi 复制。](http://a2retrosystems.com/)

Apple II Pi 只是一个简单的双面板，有几个电阻、一个电容、一个接头、一个 7404 反相器和一个通信芯片[,数量 1 是 5 美元。](http://www.jameco.com/webapp/wcs/stores/servlet/Product_10001_10001_2184034_-1)如果你已经有一个 Raspi 挂在你的工作台上，并且想为 Apple II 提供一些疯狂的硬件功能，那么你真的没有比获得这些 Apple II Pi 板更好的选择了。如果我们能找到董事会文件…

下面是苹果 II Pi 的视频，展示了 Pi 驱动的苹果的所有令人敬畏的功能。谢谢[意大利]送来这封信。

[https://www.youtube.com/embed/tbqLEU35d0E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tbqLEU35d0E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)