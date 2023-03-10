# 圆柱形物体的展开图像

> 原文：<https://hackaday.com/2013/01/14/unwrapping-images-of-cylindrical-objects/>

![unwrapping-images-of-cylindrical-objects](img/5d6eab261089cff3dd4ba955f6c6b0da.png)

这里有一个自动设置，让你[创建圆柱形物体的平面图像](http://www.diga.me.uk/360degreeCamera.html)。上面的例子显示了一个奶精，让你看到连续观察时画出的图案是什么样子。

图像捕捉装备类似于[转盘摄影设置](http://hackaday.com/2012/04/27/scanning-turntable-digitizes-objects-as-3d-models/)，允许您构建动画 GIF 文件或对象的 3D 模型。对象被放置在步进电机上，当在帧之间旋转对象时，步进电机允许精确控制。EiBotBoard(我们至少在[的另一个项目](http://hackaday.com/2012/04/18/robotic-whiteboard-writes-your-wall-on-the-wall/)中见过)是为 EggBot 打印机设计的。但它在这里被用来连接电机和捕获设备与树莓 Pi。

我们有点不确定 RPi 是否真的处理图像操作。该项目使用 ImageMagick，它肯定会在 RPi 上运行。有提到[树莓 Pi 相机](http://hackaday.com/2012/11/24/raspberry-pi-camera-board-coming-early-next-year/)加入钻机作为未来的改进，所以我们确实希望在某个时候看到全自动的修订。

【经由[阿达果](http://www.adafruit.com/blog/2013/01/11/inside-out-eggbot-piday-raspberrypi-raspberry_pi/)经由 [EMSL](http://www.evilmadscientist.com/2013/inside-out-eggbot/)