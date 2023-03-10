# 使用 OpenCV 与覆盆子 Pi

> 原文：<https://hackaday.com/2013/03/04/using-opencv-with-the-raspberry-pi/>

当我们第一次听说 Raspberry Pi 的时候，我们很高兴曾经需要一台成熟的计算机的项目现在可以在一个运行 Linux 的小而便宜的主板上完成。不幸的是，我们还没有在 Raspi 上看到太多使用计算机视觉算法的方式，但多亏了[Lentin][OpenCV 的世界现在对任何地方的 Raspberry Pi 用户都是可访问的](http://www.technolabsz.com/2013/03/how-to-easily-install-opencv-on.html)。

[Lentin]不想从源代码安装 OpenCV，这个过程要花掉一天的大部分时间。相反，他使用新立得软件包管理器来安装它。连接网络摄像头后，[Lentin] ssh 进入他的 Raspi 并安装了 OpenCV 附带的人脸检测示例脚本。

应该注意的是，[Lentin]的 OpenCV 安装速度并不快，但是对于很多项目来说，能够每秒更新五次面部追踪器已经足够了。一旦 Raspberry Pi 相机模块发布，Raspi 上的人脸检测速度应该会大幅提高，尽管如此，这将导致使用 Raspberry Pi 构建更有用的计算机视觉。