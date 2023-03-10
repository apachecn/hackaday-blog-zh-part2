# [本·克拉斯诺]黑了一台扫描电子显微镜

> 原文：<https://hackaday.com/2014/09/03/ben-krasnow-hacks-a-scanning-electron-microscope/>

[Ben Krasnow]很可能是唯一一个拥有扫描电子显微镜(SEM)收藏的黑客。[他买了一台全罗 JSM-T200](https://www.youtube.com/watch?v=SWVu-qPR-Ws) ，这在 20 世纪 80 年代早期很流行。【本】也买了一台很棒的。他只需支付从瑞典到他的车库的运费。扫描电镜实际上是在运输过程中掉落的，但谢天谢地，唯一的损坏是一个松动的阴极射线管颈塞。JSM-T200 加入了[本的][T2 的]自制 SEM、他的[T4 的 DIY CT 扫描仪、完美饼干机[和他实验室里的许多其他项目。](http://hackaday.com/2014/01/15/ben-krasnow-did-it-all-for-the-perfect-cookie/)

JSM-T200 是旧技术；从这台机器中存储图像的主要方式是通过一个屏幕安装的宝丽来相机，就像一个旧的示波器。然而，它仍然与当前的 SEM 有许多共同之处。在实时视频模式下，扫描电镜只能从目标的给定部分收集一到两个反射电子。这就产生了一个低对比度的鬼影，我们开始把它和 SEM 联系在一起。

由于电子相互排斥，试图向目标发射更多的电子将会使电子束散焦。试图从更高的电压发射电子只会将它们嵌入目标。即使是采用新技术的中小企业也不得不应对这些问题。幸运的是，有一种方法可以绕过它们。

当“写入照片”时，显微镜切换到慢速扫描模式，扫描图像一分钟。这种较慢的扫描让显微镜有额外的时间发射和收集更多的电子，从而获得更好的图像。使用这种模式，[Ben]发现他的显微镜能够产生高分辨率的数字图像。它只需要一个数字采集子系统。

点击休息时间，查看[Ben]如何更新他的显微镜！

使用原理图，[Ben]将他的 Tektronix MDO3000 系列示波器连接到他的 SEM 的视频信号。泰克很好心地把这个模型给了[本]、[达夫·琼斯]和其他几位杰出的黑客。我们也很想试一试，但我们很确定我们已经被永久列入了他们的淘气名单。

通过触发扫描电镜的垂直刷新，[Ben]能够将整个图像捕获到示波器的存储器中。他将数据导出到一个 u 盘，并将其加载到 [GNU Octave](http://www.gnu.org/software/octave/) 中，他编写了一个简单的脚本来搜索水平刷新脉冲并构建光栅图像。至少可以说，结果是惊人的。[Ben 的]能够捕捉到经典的蝇眼，而不需要像 SEM 通常要求的那样先给蝇眼镀上金属。

我们迫不及待地想知道[本]下一步会想出什么！

[https://www.youtube.com/embed/SWVu-qPR-Ws?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SWVu-qPR-Ws?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)