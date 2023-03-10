# 组合锁使用继电器和逻辑门

> 原文：<https://hackaday.com/2013/04/08/combo-lock-uses-relays-and-logic-gates/>

![logic-combo-lock](img/e8d478166de985ac57c6ac5fbef91f6e.png)

这里有一个非常有趣的电路，[使用继电器和逻辑门](http://circuit4hobby.altervista.org/electronic-key.html)实现了一个密码锁。即使有了它如何工作的示意图和书面解释，我们仍然有些茫然。这个周末，我们要么拿出一些纸来手工制作，要么在类似阿塔努阿的模拟器[中一块一块地制作。不管怎样，这个项目引起了我们足够的兴趣，以至于我们想深入了解它的内部运作。](http://hackaday.com/2008/12/18/7400-series-logic-simulator/)

从描述中我们知道它使用了 CD4017、CD4030、CD4072 和 CD4081 芯片的组合。你可能对 4017 很熟悉，这是一个在很多项目中流行的十年计数器。其他芯片分别提供 XOR、OR 和 and 门。选择继电器有两个目的。当输入正确的组合时，其中一个就会激活，有效地作为组合锁的输出。另外两个用于激活时钟，并在输入错误的组合时影响重置。

这让我们想知道，通过监听重置继电器激活的声音来暴力破解密码是否会非常简单？很难从休息后的视频中判断出你是否能仅凭声音辨别出一个错误的数字。

[https://www.youtube.com/embed/Xs8a3ElYins?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Xs8a3ElYins?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)