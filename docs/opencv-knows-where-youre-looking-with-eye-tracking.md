# OpenCV 通过眼球追踪知道你在看哪里

> 原文：<https://hackaday.com/2012/05/30/opencv-knows-where-youre-looking-with-eye-tracking/>

![](img/40bd785598583783236dd4a86592ec4c.png "eye")

[John]一直在使用 OpenCV 开发一个基于视频的眼球追踪解决方案,我们很喜欢这个进展。[约翰]的瞳孔跟踪软件可以告诉任何人你在看哪里，并允许自由移动头部。

这种构建背后基本思想很简单；直视前方时，瞳孔完全是圆形的。当眼睛看向一边时，对于安装在屏幕上的摄像机来说，瞳孔看起来越来越像一个椭圆。通过测量这个椭圆的尺寸，[约翰]的软件可以很好地猜测眼睛在看哪里。如果你想要非常技术性的分析，[这里有一篇 ACM 论文](http://www.mmk.ei.tum.de/publ/pdf/08/08koh1.pdf)回顾了这一技术。

像 [EyeWriter 项目](http://eyewriter.org/)一样，这种构建是基于【John】的构建使用监视器边缘的红外发光二极管来增加瞳孔和虹膜之间的对比度。

广告之后是两段视频，展示了眼球追踪仪的运行。看着[John]的项目工作有点令人毛骨悚然，但好消息是一个合适的眼球追踪设置不需要用户盯着他们的眼睛。

[https://www.youtube.com/embed/-B5JolF2N6s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-B5JolF2N6s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/8edm_LGQWDA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8edm_LGQWDA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)