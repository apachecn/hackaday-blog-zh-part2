# 带 Arduino 的单像素数码相机

> 原文：<https://hackaday.com/2015/01/31/a-single-pixel-digital-camera-with-arduino/>

[Jordan]设法用几个组件拼凑出他自己版本的低分辨率数码相机[。生成的图像分辨率很低，而且只有灰度，但是用一些基本的硬件所能做的事情令人印象深刻。](http://chynehome.com/web/appareil-photo-de-1-pixel-avec-un-arduino/ "Arduino digital camera")

相机的核心是图像传感器。大多数消费类数码相机都有大量的微型接收器塞在传感器里。这允许更大分辨率的图像，在更小的空间内捕捉更多细节。不幸的是，这通常意味着更高的价格。(乔丹的)传感器只有一个像素。该传感器实际上只是一个管内的红外光电二极管。二极管连接到 Arduino 上的模拟输入引脚。传感器可以指向一个物体，Arduino 可以感知这一点的亮度。

为了编译一个实际的图像，[Jordan]需要获得多个点的读数。大多数相机使用大像素阵列来实现这一点。由于(乔丹的)相机只有一个像素，他不得不移动它，一次读取一个数据。为了实现这一点，Arduino 连接了两个伺服电机。这使得传感器可以水平和垂直瞄准。Arduino 在网格中缓慢扫描传感器，沿途读取读数。 A P 处理应用 然后获取每个读数并编译最终图像。

由于这台相机编辑图像的速度太慢，它有时会出现亮度变化的问题。[Jordan]注意到了这个问题，当他拍摄图像时，云会经过。为了解决这个问题，他增加了一个环境光传感器。Arduino 可以检测整体环境光的数量，然后调整每个读数进行补偿。他说这并不完美，但结果仍然是一个进步。也许下次他可以试试彩色的[。](http://hackaday.com/2014/10/20/a-single-pixel-color-digital-camera/ "Color single pixel camera")