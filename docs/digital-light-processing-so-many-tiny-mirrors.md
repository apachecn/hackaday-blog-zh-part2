# 数字光处理，这么多小镜子

> 原文：<https://hackaday.com/2015/03/22/digital-light-processing-so-many-tiny-mirrors/>

你知道吗，在一些现代投影仪中，有一百万个小镜子来回闪烁，反射光线；像一个翻转点显示，但在微观层面？在他的视频中，[Ben Krasnow] [解释了 DLP](http://benkrasnow.blogspot.com/2015/03/how-digital-light-processing-dlp-works.html?m=1) 或*数字光处理*技术中的微小魔法，他用移动部件构建了一个按比例放大的模型。

液晶投影仪的工作原理很像老式的幻灯机。光线穿过包含图像的透明屏幕，然后通过透镜聚焦和放大。然而，DLP 投影仪以稍微不同的方式实现移动图像。一束聚焦的光线照射到一个芯片上，芯片上装有一排小得惊人的镜子。当镜子朝一个方向翻转时，它通过透镜将光线反射出去，并产生一个可见像素。当镜子向相反方向倾斜时，没有光被反射，像素是暗的。所有这些微小的移动部件都是通过静电来驱动的，由于像素实际上只能处于*开*或*关*状态，中间没有任何数值范围，像素必须以足够快的速度摆动，以实现强度的幻觉，就像脉冲 LED 以产生调光效果一样。

除了切开这些微型镜面芯片的保护外壳，让我们在显微镜下看到它们的物理表面之外，[本]还用夹在细绳之间的镜面和金属垫圈构建了自己的功能矩阵。当电流通过导线时，位于每个瓦片后面的缠绕电磁体将像素倾斜到位——尽管他没有以这种方式浪费建立完整阵列所需的时间(我们不怪他)。如果你有时间，再加上一个高功率闪光灯，这是一个在你室友的墙上展示信息的绝佳方式。

[https://www.youtube.com/embed/9nb8mM3uEIc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9nb8mM3uEIc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)