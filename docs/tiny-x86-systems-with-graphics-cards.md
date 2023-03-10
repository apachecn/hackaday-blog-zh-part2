# 带有显卡的微型 X86 系统

> 原文：<https://hackaday.com/2015/07/03/tiny-x86-systems-with-graphics-cards/>

Intel Edison 已经过时了，这意味着有人试图获得一台邮票大小的 x86 机器，运行所有那些经典的 90 年代中期游戏，而这些游戏在现代硬件上无法运行。Edison 并不是唯一一台搭载 x86 处理器的微型单板计算机；[图例讲述了另一个](https://www.youtube.com/watch?v=shlirczvcwg)，你可以连接一个显卡到这个。

这个版本使用 86Duino Zero，这是一台被塞进 Arduino 外形的单板计算机，其 CPU 的能力与奔腾 II 或 III 差不多，装载了 128 MB 的 RAM、PCI-e 总线和 USB。我们已经有一段时间没有看到 86Duino 了。我们第一次看到它是在 2013 年初，从那以后，除了这个版本之外，没有其他版本出现。

86Duino Zero 只有一个 PCI-e x1 连接器，但通过 x16 适配器，这个小小的主板可以驱动一台旧的 nVidia GT230。需要一个 Coreboot 映像的补丁和一个 VGA 复位信号的电阻，但除此之外，在 Arduino 大小的东西和明显更大的显卡上运行旧游戏并不十分困难。

感谢[Rasz]发送此邮件。

[https://www.youtube.com/embed/shlirczvcwg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/shlirczvcwg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)