# 高级超越 WiFi SD 黑客:自定义内核、X 和 Firefox

> 原文：<https://hackaday.com/2013/09/19/advanced-transcend-wifi-sd-hacking-custom-kernels-x-and-firefox/>

[Dmitry]阅读了关于破解创见 WiFi 卡的文章，并决定亲自[试一试](http://dmitry.gr/index.php?r=05.Projects&proj=15&proj=15.%20Transcend%20WiFiSD)。我们已经用超越卡介绍了[【帕布罗】的工作。[德米特里]采取了不同的方法，足以保证第二次检查。](http://hackaday.com/2013/08/12/hacking-transcend-wifi-sd-cards/)

与其从 web 界面和用户脚本开始工作，【Dmitry】决定从 [Transcend 的 GPL 包](http://www.transcend-info.com/Support/)开始，一路向上。不幸的是，他发现这个包装非常不完整——将这张卡严格归入“违反 GPL”一类。毫不畏惧，[德米特里]给支持人员发了几封电子邮件，继续坚持。

原来这个卡是用 u-boot 把内核和基本文件系统扩展成一个 ramdisk。不幸的是，这个尺寸仅限于 3MB。这个限制被硬编码到 u-boot 中，其源代码没有包含在 GPL 包中。

[Dmitry]能够在 3MB 极限内创建自己的二进制图像，并将其加载到卡上。他发现了一些非常有趣(也很可怕)的事情。闪存文件系统必须格式化为 FAT32，否则控制器会变得非常混乱。16(或 32)GB 的闪存也以读写方式安装到两个操作系统中。SD 卡上的 Linux，以及该卡碰巧插入的任何主机系统。至少可以说这是危险的。对闪存的任何写入都可能导致冲突，从而导致数据丢失，甚至文件系统完全损坏。

[Dmitry]花了更多的时间与内核版本斗争。最后他确实取得了胜利。他能够在 WiFi SD 卡的 ARMv5 控制器上启动自己的内核，并运行他想运行的任何东西。他通过在 WiFi 上使用 SSH 隧道启动 X windows forwarding 来测试系统。他甚至能让 Firefox 在 X 上运行，尽管非常慢。该卡甚至不需要在主机系统中-只需要电源和接地就可以通过 WiFi 启动和访问它。

在所有这些都完成之后，[Dmitry]终于从 Transcend 的一名支持工程师那里得到了回复。他们对遵守 GPL“不感兴趣”，他“可以自由地向任何 Linux 组织报告这一点”哎哟！这是我们很长一段时间以来看到的最漫不经心的违反 GPL 的行为之一。

**更新:**看起来创见在他们的 GPL 包中增加了 u-boot 源码。然而，[Dmitry]在注释中声明他们仍然缺少内核配置和一些模块源代码。