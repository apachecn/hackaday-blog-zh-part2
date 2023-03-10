# 不带白板的 3D 白板

> 原文：<https://hackaday.com/2012/04/26/3d-whiteboard-without-the-whiteboard/>

![](img/331b2494a76cb09d0164b023c188168b.png "3D-paint")

这个方法如此简单，而且效果如此之好，如果不是 4 月 1 日已经过去了，我们会称之为骗局。但我们相信(威廉·迈尔斯)和(郭杰钦)提出的东西是存在的，我们想要一个我们自己的。该项目是一种使用超声波传感器绘制三维图像的方法。

他们称之为 3D Paint，这很合适，因为软件界面很像最初的 MS Paint。它可以向你展示手写笔在三个轴上的移动，但它也可以组装一个立体图——那种使用红色和蓝色滤光镜的 3D——以便艺术家可以在绘制时看到 3D 渲染。

硬件依赖于三个传感器和一个触笔，它们都由 ATmega644 控制。这就是硬件(公平地说，也有一些琐碎的放大器电路)，使这成为一个令人难以置信的负担得起的设置。真正的工作，也是输入如此平滑和精确的原因，来自执行三边测量的 MATLAB 代码。如果你喜欢钻研数学，上面链接的文章会让你感兴趣。如果你是一个视觉型的学习者，请在休息后跳过演示视频。

[https://www.youtube.com/embed/mWgInUW6A8w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mWgInUW6A8w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢布鲁斯]