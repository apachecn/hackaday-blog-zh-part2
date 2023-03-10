# 燃烧的阴唇

> 原文：<https://hackaday.com/2014/03/06/the-flaming-yinlips/>

![furan-yinlips](img/21204a4acc639bca51a6f3356a97a4a2.png)

不，上面那个不是 Playstation Vita，是“Yinlips YDPG18A”便携式游戏系统。[Ian]发现闪存部门缺少他的阴唇，所以他点燃了他的烙铁。yin lips 基于 [Allwinner 孙茜](http://linux-sunxi.org/Main_Page)系列处理器，使用标准 TSOP48 封装闪存。闪存引脚排列和封装有一些标准化，因此[Ian]选择了他能找到的最大的引脚兼容芯片 Micron 的一对 256 千兆位(32 千兆字节)芯片。事实证明，拆除现有的闪光灯有点冒险，因为闪光灯是用胶水粘上去的。[伊恩]也没有他的热风枪手边，使事情变得更加有趣。小心翼翼地用刀片破坏了粘合。

原来焊接是最简单的部分。所有闪存芯片都有几何图形、管芯数、页面大小、块数、扇区大小等。该几何形状类似于硬盘驱动器中的几何形状。事实上，就像在现代硬盘驱动器中一样，系统在访问完整的存储阵列之前会读取一些基本信息。在 NAND 闪存的情况下，处理器可以访问存储器的第一页，并向闪存查询其部件号。一旦知道了零件号，就可以通过查找表来确定几何形状。[Ian]检查了 github 上的[NAND 表，所以他知道他的闪存芯片不受支持。由于将 Allwinner 处理器引导到 Linux 或 Android](https://github.com/linux-sunxi/linux-sunxi/blob/sunxi-3.0/drivers/block/sunxi_nand/src/scan/nand_id.c) 的[复杂性，该表和使用它的 NAND 驱动程序存在于几个地方。bootloader 的 axf 文件、U-Boot 和从基于 PC 的 LiveSuit flash 应用程序发送的几个 flash 应用程序二进制文件都需要修改。这些文件中的大部分被打包到一个闪存映像中。[Ian]使用 imgrepacker 打开图像，然后打开十六进制文件。他知道最初的 flash 参数表是什么样子，这是关键。他搜索了一个现有的 Micron flash 表条目，并用他的新芯片替换了这些参数。](http://rhombus-tech.net/allwinner_a10/)

修改完所有文件后，[Ian]重新打包了他的闪存映像并发送了过来。阴唇们通过在引导回路中不断重置来奖励他的努力工作。[伊恩]虽然不打算放弃。他连接到启动控制台，发现他修改的一个文件的 CRC 校验失败导致了重置。然后，他反汇编二进制发出复位。将 CRC 的返回值更改为“始终通过”修复了该问题。[Ian's]现在有一个注入胶原蛋白的阴唇，内部存储容量为 58GB。对于一个只有 2GB 内存的设备来说，这已经很不错了。