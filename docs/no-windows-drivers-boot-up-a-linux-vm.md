# 没有 Windows 驱动程序？启动一个 Linux 虚拟机！

> 原文：<https://hackaday.com/2015/08/04/no-windows-drivers-boot-up-a-linux-vm/>

[Voltagex]由于 pl 2303 USB/串行设备驱动程序有问题而受够了他的 Windows 机器上的 BSODs。不过，Linux PL2303 驱动程序工作得很好。一个弱者会简单地重启进入 Linux。相反，[Voltagex]采取了明显的变通办法:[在虚拟机中创建一个小型 Linux 发行版，将 USB 设备路由到驱动程序工作的虚拟机，然后将结果 Netcat 回 Windows](http://blog.voltagex.org/2015/07/29/fixing-a-buggy-windows-driver-with-a-virtual-machine/) 。

好吧，不太明显，但很酷。使用 Linux 系统交叉编译工具 Buildroot T1，他将虚拟机的大小降低到 32Mb 内存，甚至可以在小型笔记本电脑上轻松运行。复制虚拟机所需的一切都在 Github 上[发布。](https://github.com/voltagex/serial-vm-buildroot)

这是一个荒谬的解决方法吗？确实是的。但是当你已经有了一系列这样的工具，或者你只是想要一个学习它们的借口，为什么不呢？又有谁能放过[网猫](http://nc110.sourceforge.net/)的一个新奇用途？