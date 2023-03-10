# 袖珍串行主机充当 Apple II 磁盘驱动器

> 原文：<https://hackaday.com/2013/02/06/pocket-serial-host-acts-as-an-apple-ii-disk-drive/>

![apple-II-pocket-serial-host](img/ac382cfcb905625061b5fccf63a76b0c.png)

[Osgeld]正在炫耀他所谓的理智检查。这是他的口袋系列主机的第一个非试验版。他一直致力于这个项目，以简化他的“复古长凳”上的 Apple II 程序。插上电源后，电脑会将其视为磁盘驱动器。

存储由隐藏在原型板下侧的 SD 卡提供。这使得用现代计算机破解你的程序变得非常简单，然后把它们转移到复古的硬件上。使用的组件(从电路板的远端开始)是一个 DB9 串行连接器，旁边是一个电平转换器，使其能够与工具指向的 ATmega328 芯片进行对话。下方的芯片是一个电平转换器，用于让微控制器与右侧的 RTC 芯片对话。当安装在右上角的 5V 和 3.3V 稳压器没有供电时，电池保持时钟运行。

休息后的视频展示了这个原型，试验电路板电路，以及 Apple II 的演示。

[https://www.youtube.com/embed/RORbqhR3D6g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/RORbqhR3D6g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢布兰登]