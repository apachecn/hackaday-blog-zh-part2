# 图形计算器上的动画 gif

> 原文：<https://hackaday.com/2015/06/17/animated-gifs-on-a-graphing-calculator/>

TI-84 Plus 图形计算器配有 Z80 处理器、128 千字节内存和 96×64 分辨率灰度 LCD。你可能会认为这么瘦的机器不可能播放视频。你可能是对的。动画 gif，另一方面，它可以处理和[【searx】在这里告诉你如何](http://www.instructables.com/id/Running-Videos-on-a-TI84-Calculator/?ALLSTEPS)。

在组装他的电影之前，[searx]首先需要抓取一些视频并将其转换成 TI-84 可以显示的内容。为此，他拍摄了一段视频，并使用 Premiere Pro 将分辨率降低到 95 乘 63 像素。这些帧被保存为 BMPs，转换为单色，通过 pic9 重命名为 pic0，并上传到计算器的 RAM。

为了显示动画 GIF，[searx]编写了一个小程序，一次循环显示一幅图像。这个程序和图像本身一样，通过 USB 接口上传到计算器。播放这些动画 gif 就像调用程序，告诉它显示图像的速度，然后退后一步，在计算器上观看一个简短的电子书动画一样简单。