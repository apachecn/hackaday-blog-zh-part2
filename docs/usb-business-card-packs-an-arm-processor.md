# USB 名片包一个 ARM 处理器

> 原文：<https://hackaday.com/2012/08/24/usb-business-card-packs-an-arm-processor/>

![](img/5364f66d3c88f692fbd8e8e854549dd7.png "card")

在黑客日论坛上，[布莱恩]通过展示他的新名片来介绍自己。鉴于他的专长是制造独特的电路板，我们无法想象比 ARM 驱动的名片更好的方式来展示他的技能。

[Brian]在他的博客上发布了一篇更详细的文章[，介绍了他的开发过程。他决定使用 48 针 LPC1343 ARM Cortex M3 作为 USB 大容量存储类设备。实例化 USB 存储设备的所有繁重工作都由微控制器处理，因此[Brian]所要做的就是连接闪存芯片，并通过 SPI 接口访问它。](http://graphsandwords.com/usb_bc.html)

完成的名片功能就像一个存储容量高达 1 兆字节的 USB 拇指驱动器。这并不是很大的存储量，但对于[Brian]的简历、他的网站链接和他的名片的完整源代码来说已经绰绰有余了。