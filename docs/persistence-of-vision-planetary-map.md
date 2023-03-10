# 视觉暂留行星地图

> 原文：<https://hackaday.com/2013/11/28/persistence-of-vision-planetary-map/>

![POV planetary map](img/7289e793daddfe4692861d0742419f4f.png)

看着上面的循环 GIF，你可能会想，哦，另一个硬盘 POV 设置…嗯… [不完全是。](http://cargocollective.com/ASTRARIUM/6739848)

这是[Dev]的最新项目之一，它是一张行星地图，显示了从 1800 年到 2050 年之间任何给定日期的所有 8 个主要天体的角位置。它还能够显示模拟时钟指针、月相和其他简单的图形。

主要单元是一个硬盘，但[Dev]去掉了它的许多功能，使它看起来更加暴露，更有针对性。他使用 EagleCAD 从头开始设计 LED 轴承 PCB，eagle CAD 位于驱动器的背面，主轴穿过。它有 8 个由 5 个表面安装的 led 组成的环，通过他使用 Shapeways 打印的不透明塑料扩散环发光——它们具有小凹槽，可以紧贴在 led 上方的板上。顶层是一个 1 毫米厚的黑色圆盘，由某种未知材料制成，被[Dev]放在周围，现在在 led 的准确位置上加工了 8 个孔。

Cortex-M0 使用 LPCXpresso 板驱动 led，该板允许 led 仅跨越硬件 I/O 端口的一个字节。在软件端，磁盘的每次旋转都被分割成 360 个 1 度的切片。这个系统允许他以每秒 25 帧的速度获得 8×360 像素的圆形分辨率。对于一个视觉暂留装置来说还不错！

休息后留下来看看这款设备相当有趣的演示视频。

[https://player.vimeo.com/video/80288049](https://player.vimeo.com/video/80288049)