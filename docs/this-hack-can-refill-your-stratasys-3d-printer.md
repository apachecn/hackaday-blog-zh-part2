# 这个黑客可以填充你的 Stratasys 3D 打印机

> 原文：<https://hackaday.com/2012/09/19/this-hack-can-refill-your-stratasys-3d-printer/>

【丹】有自己的 Stratasys Dimension SST 768 3D 打印机。这是一台专业级的机器，工作非常出色。但是到了更换墨盒的时候，他不得不支付 260 美元。他可以以每公斤 50 美元的价格购买 ABS 细丝，所以他开始重新填充自己的 P400 墨盒。

重新装弹肯定很容易，因为他根本没有描述这个过程。但是填充它的物理行为并不意味着你可以继续使用它。墨盒和打印机都存储使用信息，防止这种类型的 DIY 笔芯；墨盒里有一个 EEPROM，打印机硬盘上有一个日志文件。[Dan]把硬盘拿出来，用一张 Live CD 制作了一个图像。他将映像加载到一个虚拟机中，做了一些更改以启用 SSH 并在每次启动时删除日志文件，然后将映像加载回打印机的驱动器。他写的一个脚本能够备份和重写 EEPROM 芯片，这基本上是回滚“里程表”上已经使用了多少灯丝。

[ [图像来源](http://blog.stratasys.com/blog/3d-printers-in-education/dimension-3d-printers-at-new-england-institute-of-technology)