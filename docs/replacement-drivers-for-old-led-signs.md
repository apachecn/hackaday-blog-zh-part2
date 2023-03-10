# 旧 LED 标志的替代驱动程序

> 原文：<https://hackaday.com/2013/01/11/replacement-drivers-for-old-led-signs/>

![led-sign-driver-replacement](img/6cc9b68b54c69bd47e0491f4f65e9ba6.png)

左边闲置的 LED 标志[被右边显示的 Arduino 替代驱动](http://www.bobdavis321.blogspot.com/2013/01/signature-electronic-signs-convert-to.html)激活。大的那个是 Signature Electronic 制造的，用作广告展示，就像你在商店门口看到的一样。[鲍伯·戴维斯]拿起易贝被卖为非工作。经过一些电源维修后，他开始用自己的硬件驱动它们。

他分享的图像让我们很好地了解了标志上使用的部件。显示区域由一组八个 8×5 像素的 LED 模块组成。每个模块的顶部和底部都有一个键和插槽，有助于在构建更大的阵列时正确对齐各行。他们使用 TPIC6B595 移位寄存器(与昨天低分辨率游戏黑客中看到的[相同)和 74HCT138 解码器来复用像素。这些信息大部分在](http://hackaday.com/2013/01/10/prototyping-a-low-resolution-handheld-gaming-rig/)[他帖子的第二部分](http://www.bobdavis321.blogspot.ca/2012/12/signature-electronic-sign-repair.html)分享。

他还没有得到更大的标志来正常运行。每行显示相同的数据，但比上一行低一个像素。如果你对为什么会发生这种情况有所了解，我们相信他会很乐意听到的。

[via [危险原型](http://dangerousprototypes.com/2013/01/09/signature-electronic-sign-control-board-replaced-with-arduino/)