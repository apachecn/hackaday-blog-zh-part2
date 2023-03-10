# 你的大脑认为它在燃烧你，但它不是

> 原文：<https://hackaday.com/2015/07/01/your-brain-thinks-its-burning-you-but-its-not/>

在邪教经典沙丘中，有一个虚构的装置叫做“疼痛箱”。如果你触摸它，你会觉得你的手在燃烧，但实际上，没有组织被损坏。在现实世界中，这被称为[热格栅错觉](https://en.wikipedia.org/wiki/Thermal_grill_illusion)，它早在 1896 年就被发现了。令我们懊恼的是，[亚当·戴维斯]刚刚完成了[的工作原型。](http://thermalgrill.com/)

听起来熟悉吗？几个月前，我们报道了一个类似的项目，但不幸的是，它并没有很好地运作。幸运的是，当这种情况发生时，我们很喜欢，[亚当]看到了这个帖子，并受到启发，自己尝试一下。他几年前就已经设计了一个系统，但从未着手建造。一看到这个帖子——以及让它发挥作用的困难——他就必须弄明白。

那么它是如何工作的呢？热格栅错觉使用交替的冷热条刺激你皮肤中的温度感受器——并混淆它们。无论是暖棒还是冷棒的温度都不足以造成任何伤害，但你混乱的小温度感受器让你感觉像是在燃烧或冷冻你的皮肤！

为了做到这一点，[Adam]正在使用[热电冷却器(TEC 的)](https://en.wikipedia.org/wiki/Thermoelectric_cooling)，它利用珀尔帖效应在设备的两侧产生温差。一些温度 PID 控制器确保一切都保持在安全的温度范围内——TEC 可能变得过热或过冷！最终的系统运行良好，并很好地展示了其效果；看看下面的演示就知道了。

[https://www.youtube.com/embed/otweN9sCSd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/otweN9sCSd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)