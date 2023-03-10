# 只有摄像机捕捉到的幽灵般的图像

> 原文：<https://hackaday.com/2013/07/12/ghostly-images-captured-only-on-camera/>

![is that a logo](img/cdac0fd5083072628870fafa4098ba7e.png)

不久前，我们的好朋友[Ch00f]建造了一个对人类和计算机都不可读的 QR 码时钟。由于 QR 码的数字特性，人类无法读取时钟，并且因为时钟使用视觉暂留来驱动 led，所以数码相机无法同时捕捉 QR 码中的所有像素。这是一件非常无用但令人印象深刻的艺术品。现在，【Ch00f】[正在翻转那座建筑](http://ch00ftech.com/2013/07/11/rolling-shutter-display/)。他创造了一个基本的显示器，人眼看不到，但很容易用数码相机检测到。

这种构建利用了 CMOS 数码相机的一个基本属性——滚动快门。因为从现代数字图像传感器获取像素需要时间，所以每张照片实际上是许多不同条纹的合成，每张照片的拍摄顺序都略有不同。你可以用你的照相手机拍一张旋转非常快的东西的照片来亲眼看看这一点；一张飞机螺旋桨的照片会让叶片看起来弯曲，或者看起来像[苏斯博士]有航空工程学位。

为了创造他的展示，[Ch00f]找到了一些便宜的光纤灯。通过将其中一些排列成列，并以精确的顺序点亮它们，他可以利用滚动快门，使图像出现。对于人眼来说，它看起来像一堵由照明光纤组成的实心墙。

至于这个构建的实用性如何，[Ch00f]说的不多。对于手机相机，你需要一个非常非常短的曝光时间来工作。唯一的办法就是让这个显示屏亮得令人难以置信，或者把它放在阳光下。我们看不出这对于任何潜在的用例是可行的，但是我们非常乐意看到用这种技术显示图像的大规模尝试。