# 3D 打印:扫描 3D 模型

> 原文：<https://hackaday.com/2013/08/24/3d-printering-scanning-3d-models/>

![](img/732f3581862beb942a2279d46c66e789.png)

Makerbot 数字化仪于本周发布，它让任何拥有 1400 美元的人都能够扫描小物体，并在任何 3D 打印机上打印出副本。

鉴于 Hackaday 评论和互联网上其他论坛对 Makerbot 的尖刻批评，很明显 Hackaday 的读者群和 Makerbot 开发和营销的目标人群没有交集。我们认为任何读到这里的人都宁愿卷起袖子*建造*一个 3D 扫描仪，但是从哪里开始呢？对于那些想要 3D 扫描仪但对 Makerbot 产品不太感兴趣的人来说，下面有几个选择。

Makerbot 数字化仪实际上是一个非常简单的设备。它只是一个转盘、摄像机和一对激光二极管。这是我们以前见过的带有 [DSLR 和激光笔](http://hackaday.com/2013/05/15/3d-scanner-with-remarkable-resolution/)以及[数码相机、激光水平仪和旧唱片转盘](http://hackaday.com/2010/03/18/ditch-the-lps-and-build-your-own-3d-scanner/)的东西。硬件只是这个等式的一部分——使用这种方法制作数字 3D 对象的大量工作都投入到捕捉算法中。上面的构建使用了从 MATLAB 到 Python 脚本的所有东西，所有这些都可供您阅读。

“激光和相机”方法并不是捕捉 3D 物体的唯一方法。随着小型微型投影仪的出现，一些修补者开始研究结构光扫描。这种方法记录投射到一个图像上的黑白条纹的几个图像。也有几个库可以获取这些图像，并将其转化为 Blender 可读的东西，其中最受欢迎的是[结构光库](https://code.google.com/p/structured-light/)

微软的 Kinect 在 3D 打印领域也发挥了巨大作用；最好的项目之一是 [ReconstructMe](http://reconstructme.net/) ，这是一个工具，它可以让任何装有 Kinect 的计算机充当扫描仪，至少和其他任何东西一样准确。不过，有一个问题:该软件的“专业版”售价为€180/240 美元。

当然，所有这些 3D 扫描问题的解决方案只适用于相对较小的项目。如果你想扫描更大的东西——一辆汽车甚至一栋建筑——你最好的选择可能是沿着[kincontinuous](http://www.youtube.com/watch?v=D3yYjaLmiqU)的路线。这个神奇的应用程序允许你带着 Kinect 进入战场，扫描*巨大的*区域，把它们变成可以打印的模型，或者仅仅是反恐精英的地图。

应该注意的是，Kintinous 的源代码和二进制文件都是不可用的，这要感谢对这个令人敬畏的工具背后的研究人员的一些限制。Kintinous 的论文是可用的，我们听说如果有人将他们的技术应用于一个功能性的开源项目，研究人员会很高兴。