# 无微控制器构建的 LED 蚀刻草图

> 原文：<https://hackaday.com/2013/05/23/led-etch-a-sketch-built-without-a-microcontroller/>

![logic-etch-a-sketch](img/73c4b1e53ce6d510fc179c1a72eee253.png)

这个项目是一个很好的例子，说明用一个相当复杂的逻辑电路可以完成什么。这是一个由 16×16 的 LED 栅格制成的[蚀刻草图。这本身只是有点有趣。但是当听说它的特点以及它是由逻辑芯片驱动时，我们无法想象它是如何设计的。没有示意图，但视频解说解释了一切。](http://www.youtube.com/watch?v=fxzy5kn4yzc)

最让我们困惑的是，光标比其他像素更亮。这是通过两个不同的 555 次和一个占空比技巧完成的。当你转动微调按钮时，一些十进制计数器会跟踪光标位置。路径中的像素被写入充当帧缓冲器的 RAM 芯片。甚至还有一个电平转换黑客，让显示器在 15v 下运行，以实现所需的亮度。顶级！

[https://www.youtube.com/embed/fxzy5kn4yzc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fxzy5kn4yzc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/ECE/comments/1eu55a/electronic_etch_a_sketch_using_leds_and_no/)