# 为手持收音机编写新固件

> 原文：<https://hackaday.com/2013/03/22/writing-new-firmware-for-a-handheld-radio/>

![HAM](img/6028c0e0ec743bfbde9375ab2a489873.png)

在摆弄一个便宜的手持式双频收音机时，[Lior]，又名[KK6BWA]，发现了一个类似的甚至更便宜的收音机的原理图。他意识到编程板非常容易接近，无线电微控制器的开发工具可从制造商处获得。在这些发现之后，真正要做的事情只有一件:[为 40 美元的收音机](http://www.liorelazary.com/index.php?option=com_content&view=article&id=51:hacking-the-uv3r&catid=14:baofeng-uv5r&Itemid=17)编写新的固件，并制作一个在 2 米和 70 厘米波段播放的伟大工具。

[指令](http://www.liorelazary.com/index.php?option=com_content&view=article&id=51%3Ahacking-the-uv3r&catid=14%3Abaofeng-uv5r&Itemid=17&limitstart=2)刷新这个收音机上的固件只需要一个 Arduino 和一些杂七杂八的组件。[Lior]的[uv3r 收音机的新固件](https://github.com/lelazary/UV3RMod)还没有完全完成，但他计划添加一些真正令人印象深刻的功能。像四按钮收音机的更好的用户界面、跟踪卫星的模式、数字模式和计算机控制模式都是可能的，并且在[【Lior】的项目愿望清单](https://github.com/lelazary/UV3RMod/blob/master/WISHLIST)上。

让一台 40 美元的收音机为你的 Arduino 服务已经足够酷了，但[Lior]表示，uv3r 的这种模式甚至可以更进一步:如果你有业余无线电执照，就有可能在几英里外使用 uv3r 控制 Arduino 或其他微控制器。这是一个很棒的技术，就像我们一年前看到的 [USB 电视调谐器/软件定义无线电一样。](http://hackaday.com/2012/03/20/software-defined-radio-from-a-usb-tv-capture-card/)

休息之后，您可以查看一些在 uv3r 上运行的定制软件的演示。收音机监听 DTMF 音(由 uv3r 的老大哥 uv5r 提供)，并回放一个三位数的 DTMF 音。还有一个关于[Lior]的新收音机能做什么的更详细的演示。

[https://www.youtube.com/embed/-bYRF7IxtLA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-bYRF7IxtLA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/rfNqLhF10Gc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rfNqLhF10Gc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)