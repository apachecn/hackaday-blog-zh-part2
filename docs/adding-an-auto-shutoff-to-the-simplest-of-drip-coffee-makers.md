# 给最简单的滴滤式咖啡机添加自动关闭功能

> 原文：<https://hackaday.com/2012/07/08/adding-an-auto-shutoff-to-the-simplest-of-drip-coffee-makers/>

![](img/2e9f1b2f77647e99141052ad4364949b.png "adding-a-shutoff-to-mr-coffee")

[Jerry Pommer]和他的妻子多年来一直依赖一个过滤咖啡壶。我们对带着这些东西的野营旅行有着美好的回忆；他们做的咖啡很棒，在寒冷的早晨，在森林深处喝起来味道更好。但是最近来自 stork 的一个包裹意味着他们不再有时间坐下来看咖啡。经过几天的煮沸,[杰里]改用这个非常简单的滴滤式咖啡机，这是他从垃圾堆里捡来的。它只有一个开关，除此之外什么都没有。为了确保他不会忘记关机，[他为设备](http://www.jerrypommer.com/?p=19)组装了自己的关机定时器。

他写的都是背景故事，但休息后嵌入的 34 分钟视频带我们了解黑客本身。我们喜欢他开始讨论他本可以选择的不同选项。当然，它可能是一个微控制器，或 555 定时器保持时间。但是最后他用了一个简单的电阻电容计时器。精心计算的元件对驱动达林顿晶体管，使继电器保持闭合。当缓慢消耗的电容器使电压下降超过某一阈值时，它也切断了热板的电源。在这种情况下，它只会持续大约半个小时。

[https://www.youtube.com/embed/zQ2qSlSoPYo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zQ2qSlSoPYo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)