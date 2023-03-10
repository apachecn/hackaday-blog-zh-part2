# 建造你自己的核聚变驱动器

> 原文：<https://hackaday.com/2012/11/05/building-your-own-fusion-drive/>

![](img/82765e466b5eb272728e47dbf7362c20.png "building-your-own-fusion-drive")

我们错过了最初的公告，但苹果在他们的最后一次活动中推出的不仅仅是 iPad Mini。他们有一个名为 Fusion Drive 的新存储系统，该系统将固态存储的访问速度与盘片驱动器的存储密度结合在一起。当你在表面下观察时，你真正看到的是一个硬盘驱动器，其高速缓存以固态硬盘的形式被大幅放大。从现在许多大硬盘上的 64 MB 左右的高速缓存转移到 64GB 怎么样？

你不必等待苹果来做这件事。[Patrick Stein]尝试使用命令行工具将 SSD 与物理驱动器结合起来。当然，这不是一个万能的解决方案，但这是一个很好的证明。真正使其成为可能的关键是一个底层驱动程序，它可以处理 SDD 上的缓存，同时确保数据最终能够长期存储。

[via [Engadget](http://www.engadget.com/2012/11/01/mac-pro-owner-crafts-an-example-fusion-drive/)