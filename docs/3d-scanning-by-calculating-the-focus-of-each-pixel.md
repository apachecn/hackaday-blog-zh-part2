# 通过计算每个像素的焦点进行 3D 扫描

> 原文：<https://hackaday.com/2013/06/21/3d-scanning-by-calculating-the-focus-of-each-pixel/>

![calculating-focus-to-generate-depth-map](img/b96020c0062ddfc58bc244db61efaae2.png)

我们理解[Jean]用来创建他的面部三维扫描的概念，但细节有点超出我们自己的经验。他没有使用暗室和激光线来捕捉切片，这些切片可以在以后重新组装。不，这种方法[使用不同焦距拍摄的照片](http://www.stareat.it/sp.aspx?g=3ce7bc36fb334b8d85e6900b0bdf11c3)。

想法是使用[亮度](http://en.wikipedia.org/wiki/Luminance)处理照片。它查看一个像素及其邻居，减去亮度并求和绝对值，以估计该像素的对焦情况。显然，如果你对整幅图像，以及一组从同一有利位置以不同焦距拍摄的其他图像进行这样的处理，你最终会得到一个像素深度图。

我们发现最有趣的是最终的像素保留了它们原来的颜色值。因此，在移除 cruft 后，您可以获得仍然是全彩色的 3D 扫描。

如果你想了解更多关于基于激光的 3D 扫描[，请查看这个项目](http://hackaday.com/2013/05/15/3d-scanner-with-remarkable-resolution/)。

[谢谢卢卡]