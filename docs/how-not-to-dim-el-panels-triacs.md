# 如何不暗 EL 面板，三端双向可控硅开关！

> 原文：<https://hackaday.com/2012/08/10/how-not-to-dim-el-panels-triacs/>

![](img/01f529b5d82102c1aef4e76859c14977.png "number1571")

我们都有过这样的经历:一个激动人心的绝妙想法，被画在餐巾纸上，匆忙塞进实验板，但都是徒劳。即使是最好的想法有时也会受到大量现实的影响。[Ch00f]在 ch00ftech 最近也有过类似的经历，他使用三端双向可控硅开关和一些巧妙的波形处理来调暗 EL 面板。他没有把房间里的零件扔到一边，而是走进 T2，详细分析出了什么问题。

这种方法不同于大多数 EL 驱动器调暗输出负载的方式，它不是像 PWM 控制的 led 那样斩波输出，而是三端双向可控硅开关切断波形的末端，产生难看但功率较小的输出。这种方法的问题是，当您在非零交叉期间切断波形时，会导致大量电流尖峰。这些可以对廉价的 EL 逆变器造成严重破坏，并通常引起周围的头痛。[Ch00f ]推测，他的困境可能是由于 EL 线是一个容性负载，导致电压与电流不同相。这是一个有着无数答案的工程问题，我们迫不及待地想看看他会提出什么。

查看[文章](http://ch00ftech.com/2012/08/09/method-1571-for-not-dimming-an-el-panel-triac/)中的所有“细节”(如[ch00f]所言)，因为这是关于 TRIAC 操作的很好的初级读本。如果这篇文章中没有足够的 glowy wire，你还可以看看这个声音反应[面板](http://hackaday.com/2012/05/15/building-a-sound-reactive-el-panel-and-learning-something-in-the-process/)或者 el 上的[信息指南](http://hackaday.com/2011/08/25/all-about-electroluminescence/)或者更多来自[概述](http://hackaday.com/?s=ch00f)中的【ch00f】。