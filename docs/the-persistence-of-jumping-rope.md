# 跳绳的坚持

> 原文：<https://hackaday.com/2014/04/17/the-persistence-of-jumping-rope/>

![POV Jump Rope](img/3bc5bb424865a6905629d450ebd33744.png)

[Antonio Ospite]最近开始跳绳来增加他的有氧运动，同时作为一名黑客，他决定从中获得一些额外的乐趣。他发明了 JMP 绳——[可编程跳绳。](http://ao2.it/en/blog/2014/04/16/jmp-rope-programmable-jump-rope)

他使用了与普通 [POV(视觉暂留)显示器](http://hackaday.com/2011/08/12/persistence-of-vision-helicopter-blades-with-rgb-leds/)相同的原理，但有一个很酷的转变。他设法把微控制器(一个小饰品)和电池放进了跳绳的手柄里。使用滑环系统，RGB 信号传递到包含 led 的绳索。这是一个非常巧妙的设置，他写了另一个[帖子，讲述他是如何做硬件](http://ao2.it/en/blog/2014/04/16/jmp-rope-hardware)的。

为了给他的 JMP 绳创建图像，他在他的博客上[概述了成功的 POV 图像](http://ao2.it/en/blog/2014/04/16/jmp-rope-theory-and-software)的步骤。这些包括将图像调整为圆形(duh)，减少调色板，然后使用离散转换(从极坐标到笛卡尔坐标)执行像素映射。之后，你只需要在 1D 动画中一列一列地展示你新发现的像素地图。[Antonio]将这些帧作为 RLE(游程编码)索引位图存储在微控制器上。

留下来看看他是如何做到的，以及其他一些它能做什么的很酷的例子！

![Diagram of Persistence of Vision Jump Rope](img/d4940914810a3c496b8c439f8a80bf07.png)

Diagram of Handle

从他的 JMP 绳子上得到的图像令人印象深刻——看起来就像 Firefox 是为 POV 显示而制作的！

![JMP-rope-Firefox](img/1eae9b516defeb973b7acbbfe7d098e4.png)

Firefox!

【谢谢艾伦！]