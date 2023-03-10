# 用佳能相机改装适马镜头

> 原文：<https://hackaday.com/2013/04/24/hacking-a-sigma-lens-to-work-with-a-canon-camera/>

![sigma-lens-canon-camera](img/35994f0e28e163e4160ac101b499ce5e.png)

[马丁·梅尔基奥]想在他的佳能相机上使用旧的西格玛镜头。试图这样做的问题是，相机使用的通信协议与镜头预期的不同。但是如果你不介意打开它，做一点微控制器的工作，你马上就可以使用这个镜头了。

黑客使用一个 ATtiny24 芯片、两个电阻和一个电容。你不需要做任何编码，但是你需要把固件烧到芯片上([如果你没有合适的 AVR 程序员，你可以使用 Arduino](http://hackaday.com/2009/07/15/avr-isp-programming-via-arduino/) )。镜头内有足够的空间放置附加硬件，因此在重新组装外壳后，您甚至无法看出该装置被改动过。不幸的是，看起来[马丁]没有用他添加的电子设备拍摄任何镜头的照片，但他发布的原理图应该足以让你自己完成这项工作。*T3
T5*

如果你喜欢这些类型的 DSLR 黑客，你应该尝试一些极端的东西，比如用你的现代相机使用[查看相机部件。](http://hackaday.com/2012/07/25/new-cameras-learning-old-lens-tricks/)