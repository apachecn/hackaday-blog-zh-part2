# 讨厌蓝色 M&M？使用 IPhone 的强大功能对它们进行分类！

> 原文：<https://hackaday.com/2014/12/23/hate-blue-mms-sort-them-using-the-power-of-an-iphone/>

有些人真的喜欢吃特定的 M&M 颜色……你可以花几个小时把你的 M&M 巧克力豆分类成特定颜色的堆，或者你可以[造一台机器为你做这件事。](http://www.reviewmylife.co.uk/blog/2014/12/22/high-speed-mandm-sorting-machine/)

这正是[ReviewMyLife]决定要做的，而且相当可观！他用一个旋转漏斗将 M&M 巧克力豆一个接一个地放入斜槽中，然后用 iPhone 在 M&M 落下时进行颜色识别。然后，这些信息通过蓝牙传输到 Arduino，Arduino 启动一个高速电磁闸门，迫使 M&M 进入正确的滑槽进行分拣。

对于用泡沫板热粘合在一起的原型来说，这台机器工作得出奇地好，但不用担心，他计划升级它，因为概念证明已经得到证实。他希望摆脱 iPhone，首先用树莓派取而代之，3D 打印一些零件，并巩固其电源。目前，他使用三个独立的电源为 Arduino、电磁铁和料斗电机供电——效率不是很高！

此外，它不太擅长对棕色 M&M 巧克力豆进行分类。它们看起来太像 iPhone 上橙色和阴影的混合体了。他认为在图像识别软件上做一些工作，也许一些 LED 灯可以帮助相机达到目的。

[https://www.youtube.com/embed/T1bpafUsP7Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/T1bpafUsP7Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们以前见过一些这样做的系统，包括一个[可以分类小珠子的系统](http://hackaday.com/2014/01/29/automatically-sorting-beads-by-color/)！强迫症读者会吃了你的心！