# 建造有史以来最好的自制电脑

> 原文：<https://hackaday.com/2012/09/08/building-the-best-homebrew-computer-ever/>

![](img/f0084248e0294eadca7e8926392bf6de.png "SID")

几天前当我发布了一个[自制摩托罗拉 68000 电脑壮观](http://hackaday.com/2012/09/04/homebrew-68k-extravaganza/)的时候，我简单地提到了一个由【西蒙·费伯】建造的真正壮观的自制电脑。当我发布他的 68k 板的 Youtube 演示链接时，他正在一个网站上记录架构设计、硬件和软件。[那个网站现在已经上线](http://www.ist-schlau.de) ( [缓存](http://www.ist-schlau.de.nyud.net/)如果你需要的话)现在我们都可以好好看看有史以来最好的自制电脑了。

围绕 68008 CPU 构建——比最初的 MAC、Amigas 和 TI-89 中的 68008 CPU 稍弱——西蒙的 Kiwi 计算机[具有 wazoo](http://www.ist-schlau.de/hardware.html) 之外的外围设备。雅马哈 V9990 视频显示处理器提供具有 32k 颜色的 640×480 显示器。取自 Commodore 64 的两个 SID 芯片提供立体声 chiptune 音频，一个软盘控制器、IDE/ATA 总线和 [CS8900A](http://www.cirrus.com/en/products/cs8900a.html) 以太网控制器提供你期望从一台令人敬畏的计算机得到的所有实用功能。

[在软件方面](http://www.ist-schlau.de/software.html)，【西蒙】正在运行*增强版 Basic 68k，*但是他当然不能仅仅使用 Basic 来摆弄猕猴桃上所有的酷芯片。考虑到这一点，他提出了一个基于 C 的工具链，其中包括将 [libc](http://www.gnu.org/software/libc/) 移植到 Kiwi 上。

像任何好的自制计算机项目一样，提供了所有的原理图、一点代码和一个 BOM。[Simon]目前正在(稍微)重新设计 Kiwi 的 PCB 布局，我们很高兴看到这些文件发布。有人想买奇异果印刷电路板吗？