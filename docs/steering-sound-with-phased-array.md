# 用相控阵控制声音

> 原文：<https://hackaday.com/2014/04/14/steering-sound-with-phased-array/>

![entiresystem](img/3de92b155035f0a52dc548ffb5ef787a.png)

[Edward]和[Tom]设法建造了一个真正的[相控阵扬声器系统](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/s2012/tcj26_ecs227/tcj26_ecs227/index.html)能够在房间内控制声音。由 Atmega 644 供电，这个令人印象深刻的最终项目使用了 12 个独立可控的扬声器，每个扬声器都有可变的延迟。通过以精确的时间间隔调整延迟，可以改变输出波的最大强度的角度，从而“控制”声音。

[相控阵](http://en.wikipedia.org/wiki/Phased_array)通常与电磁应用相关，[如雷达](http://hackaday.com/2014/02/24/guest-post-try-radar-for-your-next-project/)。但是同样的原理可以应用于声音波形。数学有点可怕，但我们会带你了解你需要知道的东西，以防你需要用~~扬声器和伺服~~相控阵音响系统来控制声音。

相控阵系统的物理原理可以用衍射光栅来演示。

![Doubleslit3Dspectrum](img/4d64768b25b090ca351254245e236016.png)

上面的动画显示了波形通过障碍物开口时发生的情况。通过计算开口的数量，获得开口之间的距离，并将这一知识与输入波形的特性相结合，可以找到最强的区域。

![PhasedArray](img/6f081b71104d0b8ef5e8ad8f4ae8767e.png)

这是相控阵设置。如果你把每个演讲者都看作是开场白，你可以运用同样的技巧。[Edward]和[Tom]经过反复推敲，发现输出强度可以通过以下等式计算:

![Untitled](img/631d9b89f76df8b54d5d4761b6966c12.png)

其中 vs =声速，d =扬声器之间的距离，td =时间延迟。通过改变时间延迟，可以改变最大强度的角度。[Edward]和[Tom]在 MATLAB 中测试了他们的理论，结果成功了！

下面是没有延迟的几个频率的理论输出。

![zerodegrees](img/1f57127f96641d6d0407ff47d7355185.png)

这是 3ms 延迟后的输出。

![15degrees](img/f9dfb96bda5e2f7787e9faab20485b89.png)

请务必查看[Edward]和[Tom]的项目，以了解完整的详细信息、源代码、原理图等。下面是一个展示项目实时工作的视频。

[https://www.youtube.com/embed/_rb7onpgf1g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_rb7onpgf1g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)