# 损坏的光盘驱动器中的 PCB 搅拌器

> 原文：<https://hackaday.com/2013/09/10/pcb-agitator-from-a-broken-cd-rom-drive/>

![pcb-agitator](img/6ed4d85484627eff50cc87f742e59950.png)

如果你搅动溶液以带走溶解的铜并使新的蚀刻剂到达该区域，蚀刻 PCB 会进行得更好。考虑到这一点，[Rohit Gupta]在意识到他正在艰难地进行这项工作之前，在草图上设计了一个机制。他最终把他的搅拌器建立在一个坏掉的光盘驱动器上，而不是从零开始。

他使用驱动器上的 CD 滑板，抛弃了镜头及其支撑结构。为了直接访问驱动托盘的电机，他使用了 L293D H 桥芯片。这由 MSP430G2231 微控制器控制。右上角所示的驱动板包括一个稳压器、三个状态 led 和一个用户输入开关。一旦被触发，雪橇将来回移动，接触一个旧的鼠标微动开关，该微动开关充当限位开关。我们发现[Rohit]在试验板上制作电路原型，然后利用这一成功来蚀刻最终的电路板(如下面的视频所示)非常有趣。

如果你一直遵循黑客信条，从不丢弃任何垃圾，那么找到一个捐赠人来制作一个你自己的垃圾是没有问题的。但是以防万一你不能得到这个硬件[可以使用业余爱好伺服](http://hackaday.com/2009/08/15/etching-agitator/)建立一个类似的搅拌器。

[https://www.youtube.com/embed/wOFcjrQe-is?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wOFcjrQe-is?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)