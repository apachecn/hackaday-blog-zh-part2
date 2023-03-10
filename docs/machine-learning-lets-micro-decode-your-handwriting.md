# 机器学习让微解码你的笔迹

> 原文：<https://hackaday.com/2012/05/03/machine-learning-lets-micro-decode-your-handwriting/>

![](img/35eae61ca04575ad48d5d3254ea79606.png "handwriting-decoder")

这个装置会把你用手写笔写在触摸板上的字母[转化成数字字符](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/s2012/shw46_jec324/shw46_jec324/index.html)。该系统速度非常快，显示出近乎完美的识别能力。这都要归功于通过机器学习收集的大量数据集。

驱动该系统的 ATmega644 没有足够的速度和马力来独立可靠地识别笔迹。但是给它提供一个可以比较的数据集，你就成功了。[Justin]和[Stephen]设计了一种神经网络算法，该算法采用了大量的字符笔迹样本，并将它们浓缩成一组相关性，当遇到新条目时可以参考这些相关性。该设置大约为 88 千字节，对于存储在微处理器中来说太多了，但是很容易从外部闪存设备中引用。

在上面链接的文章中有大量的细节，但你可能想从休息后的视频概述开始。

[https://www.youtube.com/embed/z7HwuC4YcKA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/z7HwuC4YcKA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)