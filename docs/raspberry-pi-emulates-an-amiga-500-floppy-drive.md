# Raspberry Pi 模拟 Amiga 500 软盘驱动器

> 原文：<https://hackaday.com/2013/11/26/raspberry-pi-emulates-an-amiga-500-floppy-drive/>

[Maurizio]喜欢用他的 Amiga 500。他的经典硬件多年来一直为他服务，除了软驱，它最近坏了。对[Maurizio]来说没有问题，他只是打开了他的箱子，添加了一个 [Raspberry Pi 作为实时软盘仿真器](http://amigadrive.blogspot.it/)。[Maurizio]不想对他的 A500 机箱做任何永久性的改动，更重要的是，他想使用 Amiga 原来的软驱接口。后者对他的设计提出了一些相当严格的时间要求。

接口硬件相对简单。大部分电路专用于从 5v Amiga 500 到 3.3V Raspberry Pi 的电平转换。74LS06 Hex 逆变器将信号转换为 A500 所需的集电极开路输出。[Maurizio]从 Amiga 的软式电源连接器为他的 Raspberry Pi 供电。他的 A 型 Raspberry Pi 工作正常，但 B 型会比 Amiga 软盘电源能够提供的功率(550ma)多一点(700ma)。等式的用户界面端很简单:两个按钮，一个用于切换磁盘，一个用于“写入 SD”。实时磁盘映像存储在 Raspberry Pi 的 ram 中，因此用户需要点击“写入 SD”按钮，在交换软盘之前将任何更改存储到磁盘中。

软件可能是这个版本中最有趣的部分。[Maurizio]正在实时模拟软盘驱动器，这意味着实时模拟 [MFM 编码](http://en.wikipedia.org/wiki/Modified_Frequency_Modulation)。呼叫必须以 2 微秒的时间精度进行。Pi 的股票 Linux 操作系统只是不打算削减它。[Maurizio]编写了他的驱动仿真器[【裸机】](http://www.raspberrypi.org/phpBB3/viewforum.php?f=72)，直接访问 Raspberry Pi 上的 Arm 处理器。这使他能够访问整个处理器，并允许他满足软盘接口的严格定时要求。

[https://www.youtube.com/embed/uG8lcDisK7o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uG8lcDisK7o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)