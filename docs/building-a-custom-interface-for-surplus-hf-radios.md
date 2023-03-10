# 为剩余高频无线电建立定制接口

> 原文：<https://hackaday.com/2012/07/26/building-a-custom-interface-for-surplus-hf-radios/>

![](img/81d912dd7fcef59d8f2fdccc1f0359e0.png "custom-hf-radio-interface")

从易贝收到一台摩托罗拉 Micom 收音机。这些是美国国务院的剩余产品，但显然 125 瓦的高频单元是顶级的，价格只有标价的十分之一。一个棘手的问题是它们是无头的；没有额外的硬件你无法控制它们。但是互联网通常对爱好者很友好，这也不例外。多亏了 Micom Yahoo Group，你可以从个人电脑上下载运行收音机的软件。[PRC148]以该软件为例，构建了自己的独立接口。[ [页面的缓存版本](http://webcache.googleusercontent.com/search?q=cache:vIlDTn0TGTMJ:www.p25.ca/archive/index.php/t-399.html)

主机是一个 Arduino，驱动一个四线 LCD 显示器和一个相当大的按钮阵列。上面链接的论坛帖子展示了他在一块试验板上卑微的出身。在这个项目中，[PRC148]学到了很多技巧，最终得到了你在上面看到的东西。隐藏在重复使用的挡板后面的是他用 Eagle CAD 设计并自己蚀刻的 PCB。这使他能够将触觉开关塞得足够近，以便与键盘上的按钮覆盖层配合工作。

**更新:** 这个功能的流量把托管内容的论坛拿下来了。他们要求我们不要因为这个链接到他们。多亏了[Termm]，可以在上面找到没有图像的缓存版本。