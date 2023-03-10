# 大规模并行 CPU 处理 256 种灰度

> 原文：<https://hackaday.com/2013/02/26/massively-parallel-cpu-processes-256-shades-of-gray/>

![256](img/0dedde270def231d0f74630cf5d8fc7c.png)

20 世纪 80 年代是奇怪的计算机架构的全盛时期；许多公司尝试了奇怪的并行设计，而不是你在今天的台式计算机中找到的冯·诺依曼架构或微控制器的哈佛架构。虽然今天使用不多，但在当时，这些是他们那个时代最强大的计算机之一，并被用作 20 世纪 80 年代人工智能复兴的主要研究工具。

在挪威科技大学，一大群学生(13 名成员！)设计了大规模并行计算机的现代版本。它被称为 [256 灰度](http://www.256shadesofgray.com/index.html)，它可以处理 320×240 像素的 8 位灰度图形，这是任何微控制器都无法做到的。

该项目的想法是创建一个基于阵列的并行图像处理器，其架构类似于美国宇航局以前使用的[固特异 MPP](http://en.wikipedia.org/wiki/Goodyear_MPP) 或侏罗纪公园控制室中发现的[连接机](http://en.wikipedia.org/wiki/Connection_Machine)。与这些早期的计算机不同，该团队在 FPGA 中实现了他们的阵列处理器，从而产生了他们的 [Lena 处理器](http://www.256shadesofgray.com/lena.html)该处理器反过来由带有定制 VGA 输出的 32 位 AVR 微控制器控制。

整机每秒可处理 10 帧 320×240 分辨率的灰度视频。有一个[演示视频](https://www.youtube.com/watch?v=pOXzD_7pL4M)(挪威语)，但最精彩的可能是[他们在电脑上实时呈现的生命游戏的演示](https://www.youtube.com/watch?v=pOXzD_7pL4M&feature=youtu.be&t=4m51s)。一个令人敬畏的构建，和一个非常酷的经验，为所有的阶级成员。