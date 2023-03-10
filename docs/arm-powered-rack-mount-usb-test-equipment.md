# ARM 供电的机架安装 USB 测试设备

> 原文：<https://hackaday.com/2012/12/13/arm-powered-rack-mount-usb-test-equipment/>

![developing-rack-mount-pcb-testing-tools](img/7c64d32e1dfc54b8cc8e6f5393141720.png)

这是[林普金]在日常工作中开发的一种装置。这是一个用于物理实验的高速测试接口。我们发现它很有趣，因为[它使用 ARM 微控制器通过 USB](http://www.limpkin.fr/index.php?post/2012/12/04/ATSAM3U-SDCard-USB-CDC/MSD-FAT32-with-AT91LIB-Chan-s-fat-code) 实现 CDC 和 MSD。

该设计分为两部分，使其能够在机架安装的情况下工作。那个白色的大连接器允许交换卡。你可以看到右边的板有一个 USB-A 连接器。插入后，它将枚举为控制设备(CDC)和大容量存储设备(MSD ),使用 fat32 作为文件系统。

该平台的开发考虑到了开放硬件和开源软件。如果你正在做一个使用这些 USB 功能的项目，这是一个很好的参考。他使用的 ARM Cortex-M3 芯片是 AT91SAM3U，但将代码移植到其他类似功能的 ARM 处理器应该不会太难。