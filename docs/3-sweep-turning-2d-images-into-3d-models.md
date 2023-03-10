# 3-Sweep:将 2D 图像转换为 3D 模型

> 原文：<https://hackaday.com/2013/09/12/3-sweep-turning-2d-images-into-3d-models/>

随着 3D 打印的不断发展，人们正在开发越来越多的方法来获得 3D 模型。从基于硬件的扫描仪(如微软 Kinect)到基于软件的扫描仪(如 123D Catch ),有很多方法可以从一系列图像中创建 3D 模型。但是，如果你可以用一张*单个*图像制作一个 3D 模型，那会怎么样呢？听起来很疯狂？也许不是。一组研究人员创造了 3-Sweep，这是一种交互式[技术，用于将 2D 图像中的物体转化为可以操纵的 3D 模型](http://www.faculty.idc.ac.il/arik/site/3Sweep.asp)。

明确地说，识别单幅图像中的 3D 组件对于计算机算法来说有点力不从心。但是，通过将人的认知能力与计算机的计算精度结合起来，他们已经能够创建一个非常简单的提取 3D 模型的工具。这是通过勾勒形状来完成的，类似于人们可能在 CAD 包中建模的方式——一旦轮廓完成，算法就会接管并创建模型。

该软件在 2013 年亚洲 Siggraph 展会上首次亮相，并在互联网上引起了不小的轰动。休息后观看演示软件过程的精彩视频！

[https://www.youtube.com/embed/Oie1ZXWceqM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Oie1ZXWceqM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/oculus/comments/1m1968/xpost_3sweep_extracting_editable_objects_from_a/)