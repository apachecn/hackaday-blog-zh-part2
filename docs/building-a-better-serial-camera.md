# 构建更好的串行摄像机

> 原文：<https://hackaday.com/2013/11/12/building-a-better-serial-camera/>

如果你的下一个项目与相机或机器视觉有关，你可能会看到类似连接到 ARM 板或上网本的 USB 网络摄像头。不过，有时候，这种设置打击会让你的预算(电力或其他方面)大打折扣。对于小型项目，你只能使用小型的串行相机，在这个领域，你真的没有太多的选择。

[Ibrahim]意识到最便宜的系列相机大约 35 美元，而基本的图像处理成本飙升至大约 100 美元。他着手[制造自己的替代产品](http://sigalrm.blogspot.com/2013/07/in-search-of-better-serial-camera-module.html)，最终得到了一个非常棒的串行相机模块，数量上应该只需要大约 15 美元。

该模块围绕一个运行频率为 168 MHz 的 STM32F4 微控制器构建。这种微型有一个 DCMI 端口，一个 OV9650 相机连接。分辨率最终达到 1280×1024，远优于其他系列相机。

[易卜拉欣]已经有了工作的硬件和一些演示应用程序。他有一个实时颜色跟踪演示(下面的视频)正在运行，还有一个机器视觉 repo 用于他的微型相机。如果我们能在 Tindie 上找到几块这样的板子。

[https://www.youtube.com/embed/63_mOyZeNng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/63_mOyZeNng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)