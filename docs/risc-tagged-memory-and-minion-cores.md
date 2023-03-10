# RISC、标记内存和 Minion 内核

> 原文：<https://hackaday.com/2014/12/21/risc-tagged-memory-and-minion-cores/>

如今购买一台计算设备，你得到的可能是 x86 或 ARM。通用计算的架构不止一种，有双核 MIPS 主板可用，一些非常奇怪的芯片正在进入开发主板。lowRISC 是一些著名的芯片设计师的最新成果，能够“很好地”运行 Linux，并增加了一些以前没有以这种方式组合在一起的新颖的安全功能。

有两个有趣的特性使 lowRISC 引人注目。第一个是[标记内存](http://en.wikipedia.org/wiki/Tagged_architecture)。这种方法以前曾被用在更老、更奇怪的计算机上，作为一种内存元数据。基本上，每个内存地址的几个位将每个内存地址标记为可执行/不可执行，充当内存观察点、垃圾收集和每个字的锁。ISA 中增加了新的指令，允许对这些标签进行操作、监视和监控，以防止最常见的单一安全问题:缓冲区溢出。这是标记记忆的一个非常有趣的应用，在现代建筑中是找不到的。

下层社会的第二个特征是奴才。这些是绑定到处理器 I/O 的可编程设备，其工作方式很像一个 [Zynq SOC](http://www.xilinx.com/products/silicon-devices/soc/zynq-7000.html) 或 BeagleBone 内部的 PRU。基本上，它们用于可编程 I/O，在软件中实现 SPI/I2C/I2S/SDIO，从主内核卸载工作，以及需要非常精确时序的器件。

lowRISC 团队目前的目标是在 FPGA 上开发硬件，在一年时间内发布一些测试硅。第一个完整的芯片将是嵌入式 SOC，有望在 2016 年底或 2017 年初发布。最终目标是一个带有 GPU 的 SOC，可用于移动电话、机顶盒以及 Raspi 和 BeagleBone 类型的开发板。这个团队有足够多的人，包括剑桥大学和 Raspberry Pi 的[Robert]和[Alex Bradbury]，加州大学伯克利分校的研究人员，以及[Bunnie Huang]。

这是一个仍处于起步阶段的项目，但这些人追求的功能非常有趣，而且是其他平台所没有的。

[Alex Bardbury]去年 10 月在 ORConf 做了一个关于 lowRISC 的演讲。你可以在这里查看[的介绍](https://speakerdeck.com/asb/lowrisc-a-first-look)。