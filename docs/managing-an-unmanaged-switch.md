# 管理未被管理的交换机

> 原文：<https://hackaday.com/2015/09/07/managing-an-unmanaged-switch/>

网络交换机有两种不同的类型:管理型，通过某种接口来配置和监控设备；非管理型，设备只是做它应该做的事情，而你无法真正控制它。[Tiziano Bacocco]想要管理他廉价的非托管交换机，所以他做了任何优秀黑客都会做的事情:他打开了它。

在 Digicom 10/100 交换机内部，他发现了一个 IP178CH 控制器 IC，快速搜索后找到了一份数据手册。[Tiziano]注意到有三种方式来配置开关:一些硬件引脚可以控制非常基本的功能；EEPROM(PCB 上没有)可以配置器件；或者芯片将通过同步串行端口接受命令。

由于数据表涵盖了所需的协议，【Tiziano】[征用了一台 Arduino Pro Mini，并使用它来发送命令以配置交换机](http://linuxehacking.blogspot.it/2015/08/convert-your-unmanaged-to-vlan-capable.html)。几个电阻和一些快速代码使他能够通过 USB 端口控制 VLAN 和交换机上的其他功能。当然，他提到如果你想要一个网络接口，你可以使用一个树莓派，或者这可能是一个使用你在 Radio Shack 获得许可的以太网屏蔽的好借口。

如果您不清楚为什么关注受控交换机，请观看下面的视频。当然，你的交换机可能不使用 IP178CH，但我们在之前也报道过 TL-SG1005D 芯片的类似攻击[。](http://hackaday.com/2010/05/26/unlocking-the-crippled-potential-of-an-unmanaged-switch/)

[https://www.youtube.com/embed/CPoMG9DjY3o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CPoMG9DjY3o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)