# [Afrotech]D 类放大器指南

> 原文：<https://hackaday.com/2014/06/09/afrotechs-guide-to-class-d-amplifiers/>

![classd](img/c00a458394a2c312e52a7878e13c09fd.png)

在任何一个吉他或音响发烧友论坛或讨论区逗留足够长的时间，最终你会遇到关于放大器拓扑结构的争论。d 类放大器是这些放大器中更有趣、更有用的一类，它们效率极高，如果设计得当，听起来会相当不错。[【Afrotech】在这里向您展示它们是如何工作的](http://www.youtube.com/watch?v=O1UagNkcxi4)，以及如何使用一个 3 美元的 d 类放大器芯片构建一个 15 瓦的放大器。

放大器的定义就是将低功率信号转换成高功率信号。快速调制高功率信号的一个好方法是用脉宽调制来调制方波。d 类放大器接收低功率输入信号，用它来调制高功率方波的占空比，稍加滤波后，放大低功率输入。

为了演示这一点，[Afrotech]使用了 [TI 的 TPA3122 类放大器芯片](http://www.ti.com/product/tpa3122d2)。作为一个 15 瓦的立体声放大器，这是一个非常便宜的芯片，而且电路非常简单，可以在试验板上构建。通过几个电容、电阻和一对电感，[Afrotech]构建了这个单芯片放大器，能够为一些相当大的扬声器供电。它还非常高效，不需要散热器。

虽然 d 类放大器效率极高。有一些人说，因为放大器基本上是一个滤波方波，所以您将能够听到 a 类或 ab 类放大器的音频差异。这导致了 t 类放大器的发展，基本上是一种具有更高开关速度的 d 类放大器(t 类为兆赫，d 类为几百千赫)。尽管如此，如果你需要一个便宜的放大器，用于 DIY 音箱或任何其他高功率应用，你可以做得比简单的 d 类放大器差得多。

[https://www.youtube.com/embed/O1UagNkcxi4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/O1UagNkcxi4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)