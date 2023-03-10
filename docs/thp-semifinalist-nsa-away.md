# THP 半决赛:国安局客场

> 原文：<https://hackaday.com/2014/09/26/thp-semifinalist-nsa-away/>

回到我们创办黑客日奖的时候，安全、老大哥和国家安全局每天都是头条新闻。从那时起，新闻中已经有足够的面包和马戏来消除这些泄露的后果，但世界各地的黑客和修补者仍在努力给你提供保护数据的工具。

[NSA Away](http://hackaday.io/project/1569-NSA-Away) 就是这些工具之一。该项目的第一部分是一个独立的密钥生成器，它可以同时向一对 SD 卡写入相同的随机位。用他们的随机数发生器，这是完美的加密。破解团队用于加密的一次性密码本的唯一方法是 1)多次使用密码本的某些部分，2)有一个可怕的 RNG，或者 3)做一些非常愚蠢的事情，比如[在商店里卖一次性密码本](http://store.hackaday.com/products/1407981609)。

构建的另一部分是基于 Android 的加密设备，带有摄像头、键盘、SD 读卡器和 USB 端口。该设备读取“OTP SD 卡”,并使用 OCR 读取相机数据，然后在屏幕上解密。只要 OTP 不落入坏人之手，这是一种向任何人传输数据的绝对安全的方法。

就进展而言，团队成员有一个全功能的 pad 生成器，将随机数据写入 SD 卡。如果您想通过不安全的介质传输您的 pad，该设备还可以作为 USB HID 设备向计算机输出随机位。

这是一项令人印象深刻的工作，尤其是在 RNG 部门。该团队在电路描述中使用了八个雪崩噪声发生器。构建的这一部分还没有完全工作，但是这对于概念验证来说确实是不需要的。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客日奖的四分之一决赛。](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)**