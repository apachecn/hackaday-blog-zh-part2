# 为你的莱昂内尔火车 DIY 钟

> 原文：<https://hackaday.com/2014/03/04/diy-bell-for-your-trains-of-lionel/>

![](img/ed6d12beffc62a3c577a10153e44e109.png)【Peter】的父亲最近重新点燃了他对莱昂内尔火车的热爱，他想要一个铃铛来保证过道口的火车司机和行人的安全。在他父亲的要求下，彼得利用他到处乱放的零件和五金店的门铃，发明了这个 [DIY 火车过街铃](http://www.instructables.com/id/DIY-train-crossing-bell/)。

这个想法是让钟每秒钟响一次。为了实现这一点，[Peter]使用了一种不重复的电子机械门铃，连续按压即可发出一个音符。你也可以用弹簧螺线管和类似钟的东西来摇你自己的钟。

[Peter]的三级设计使用全波桥式整流器将列车变压器的交流电转换到 DC。他将其降至 5V，并通过 555 和一些电阻来设置频率和占空比。他的输出部分将电压向上转换，以匹配门铃所需的输入。[Peter]包括一个 1N4002 作为反电动势缓冲器，防止反馈损坏功率 MOSFET。跳伞后留下来观看他的演示视频。

[https://www.youtube.com/embed/Uw7qG2nyPrM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Uw7qG2nyPrM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)