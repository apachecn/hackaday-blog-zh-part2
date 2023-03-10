# 一种快速易用的视觉传感器

> 原文：<https://hackaday.com/2013/08/21/a-fast-and-easy-to-use-vision-sensor/>

[![](img/1f81d9b9542fad8fe193cdf90c2216c8.png)](http://hackaday.com/wp-content/uploads/2013/08/pixie.png)

在 Hackaday 上，我们不经常展示 kickstarter 活动，但在我们看来，这一次值得注意。它被称为 [Pixy](http://www.kickstarter.com/projects/254449872/pixy-cmucam5-a-fast-easy-to-use-vision-sensor) ，这是一个大约有名片一半大小的小相机板，可以检测你“训练”它检测的对象。

训练是通过将物体放在 Pixy 的镜头前并按下按钮来完成的。Pixy 然后使用专用的双核处理器以每秒 50 帧的速度处理图像，找到具有相似颜色签名的对象。Pixy 可以通过以下几种接口之一报告其发现，包括所有探测到的物体的大小和位置:UART 串行、SPI、I2C、数字或模拟 I/O

该平台是开放的硬件，其固件是开源的和 GPL 许可的，这使得该项目非常有趣。它基于 204MHz 双核 ARM cortex M4 & M0，使用 1280×800 图像传感器，可以将处理后的相机输出传输到您的计算机。你可以花 59 美元在 kickstarter 活动中得到一个精灵，这并不算贵。