# 通过 FPGA 实现基于摄像头的触摸屏输入

> 原文：<https://hackaday.com/2013/05/20/camera-based-touchscreen-input-via-an-fpga/>

![piano-hero-uses-camera-based-touch-input](img/0d96e2fe1f61d1978e9493242ed81baa.png)

[李崇刚]来信分享了他和[胡然]为他们的嵌入式系统课程制作的最终项目的链接。它被称为钢琴英雄，[使用 FPGA 来实现基于摄像头的触摸屏系统](http://people.ece.cornell.edu/land/courses/ece5760/FinalProjects/s2013/cl972_rh523/cl972_rh523/index.html)。

上面显示了项目中使用的所有硬件。显示器充当键盘，使用 FPGA 板产生的图像来标记每个虚拟键的位置。它使用常规 VGA 显示器，因此他们需要找到一些方法来监控触摸输入。该解决方案使用一个以钝角安装在屏幕上方的摄像头。也就是说，屏幕向后倾斜一点点，这样相机就可以看到屏幕上的图像。FPGA 板处理传入的图像，当您的手指在监视器和摄像头之间经过时，记录下按键。这种技术将输入限制在单行键上。

这应该比使用 CCD 扫描仪传感器的[简单得多，但是可以跟踪二维触摸输入。](http://hackaday.com/2011/03/21/converting-a-scanner-into-a-touchscreen/)

[https://www.youtube.com/embed/PimshzlagvI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PimshzlagvI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)