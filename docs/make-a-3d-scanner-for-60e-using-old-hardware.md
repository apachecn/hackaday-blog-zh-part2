# 使用旧硬件制作 60€的 3D 扫描仪

> 原文：<https://hackaday.com/2014/04/20/make-a-3d-scanner-for-60e-using-old-hardware/>

![3d laser scanner](img/7f55c5951085d06d6fac5fab16c0ca4c.png)

[蒂尔·汉德尔]刚刚完成了他写的一篇论文的最后润色，这篇论文是关于如何建造一台便宜的 3D 扫描仪——主要是用备件。

利用旧打印机和笔记本的零件，他拼凑了这个看起来相当粗糙的激光扫描仪。但是不要被它的外表所迷惑！它能够在 0.3-5 米的距离内 360 度扫描周围，是扫描房间的绝佳选择。

它使用线激光器和安装在步进电机驱动的臂上的网络摄像头，看起来像是旧的光驱。Arduino Uno 和 A4988POW 步进驱动器控制系统。[论文](http://alicedownthecoffeepot.files.wordpress.com/2011/09/documentation_laser_scanner1.pdf)(注意:PDF)非常详细，发表在 [GPLv3](https://www.gnu.org/copyleft/gpl.html) (通用公共许可证)下。

它的工作原理与许多 3D 扫描仪相同——线激光提供相机拾取的被扫描物体的 2D 轮廓。当系统(或物体)旋转时，新的轮廓被记录并缝合在一起以形成完整的 3D 图像。

![3d laser scanner diagram](img/8d1905682a092edfe599b909aa4c7429.png)

为了提高扫描仪的分辨率和精确度，你可以在最后放一个更好的摄像头！