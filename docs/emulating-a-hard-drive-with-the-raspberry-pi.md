# 用 Raspberry Pi 模拟硬盘

> 原文：<https://hackaday.com/2015/08/11/emulating-a-hard-drive-with-the-raspberry-pi/>

[Chris]最近将一台老式 IBM 5150(最初的个人电脑)搬进了他的客厅。虽然对于不属于 Hackaday 读者群的人来说，这听起来很奇怪，但实际上很有意义；这台电脑是一个伟大的无分心写作工作站，老式游戏机，看起来真的，真的很酷。它闲置了一段时间，只是因为[Chris]不想换出成堆的软盘，而且他没有这台机器的硬盘或控制卡。在回顾了其他 retrocomputer 爱好者在这种情况下所做的工作后，[他用树莓 Pi](http://www.insentricity.com/a.cl/244/adding-a-hard-drive-to-an-original-ibm-pc-using-a-raspberry-pi) 模拟了一个硬盘。

“没有硬盘的旧电脑”问题的传统解决方案是[x ide 项目](http://www.vintage-computer.com/vcforum/showthread.php?26393-XTIDE-project)。XTIDE 是一种控制器卡，它将相对较新的 IDE 卡(或另一台计算机上的模拟驱动器)转换为老式 PC 上的硬盘，就像控制器卡一样。由于一个驱动器可以被另一台计算机模拟，[Chris]抓起他手头最近的单板计算机，在这种情况下是一台 Raspberry Pi。

在用 XTIDE 烧了一个 EPROM 来驱动一个旧的网卡之后，[Chris]开始着手在 Raspberry Pi 方面开发 XTIDE 软件功能。现代版的硬件只是一个 Pi 和一个 USB 转 RS232 适配器，设置为非常低的比特率。虽然模拟驱动器很慢，但对于这个时代的计算机来说，它是相当大的:500 兆的空闲空间。想到你可以在那上面安装多少经典游戏和应用程序，你就会头晕目眩！