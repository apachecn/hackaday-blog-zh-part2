# 逆向工程 Solari 软襟翼显示器

> 原文：<https://hackaday.com/2012/10/17/reverse-engineering-solari-soft-flap-displays/>

![](img/7ea47998900414035eddd321b24e4e9f.png "solari-soft-flap-displays")

这是一个角色索拉里软式襟翼模块内部的侧视图。这是一些交通枢纽使用的机械显示器，每个字母都有一个翻盖。马达转动翻板通过字母表，直到它到达目标字母。最近,[Boz]有一个客户找到他，他需要为 20 个字符的软翻盖显示器定制一个控制器。(链接 2022 年修复。感谢 Wayback 机器！)

这个过程从放大镜和万用表开始，产生了一个相当复杂的手绘示意图。光学编码器用于判断当前显示的是哪个字符。在使用示波器分析了输出之后，Boz 设计了一个基于 PIC 的驱动板，它控制着在中断之后的剪辑中看到的显示。

这些显示器的伟大之处在于，除了改变字母之外，它们不使用任何电力。这听起来像是 ePaper 的前身，让我们想知道是否有任何公司正在开发高对比度的 ePaper 来取代软瓣手指？

[https://www.youtube.com/embed/0RbSmVLwNr4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0RbSmVLwNr4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)