# 使用 Android 设备进行人脸跟踪

> 原文：<https://hackaday.com/2012/10/15/face-tracking-with-an-android-device/>

![](img/c11206a3fde83c4bc7add9ebb81585e1.png "facial-tracking-on-android")

这款 [Android 设备可以识别人脸，并移动以将它们保持在帧](https://trandi.wordpress.com/2012/10/13/physical-face-following-with-opencv-on-android/)中。这是一个概念验证，使用常见的可用部件和软件包。

该项目的最初动机是[Dan O]想尝试 OpenCV 软件。OpenCV 是一个开源的计算机视觉包，在识别图像的含义时，它承担了主要的工作。为了让手机有动力移动，他设计并打印了自己的手机安装支架和几个业余爱好伺服系统。一个 IOIO 板连接到 Android 设备，以控制电机。在软件方面，所有[Dan]需要做的就是编写一些代码，将 OpenCV 人脸跟踪模块的输出与 IOIO 的输入连接起来。跳转后查看完成的项目演示。

这个系统可以很容易地用其他硬件实现，比如今年早些时候我们看到的这个基于 Arduino 的版本。

[https://www.youtube.com/embed/-ScAz-u5mTY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-ScAz-u5mTY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)