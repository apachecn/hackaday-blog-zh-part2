# 易于阅读的自行车电脑

> 原文：<https://hackaday.com/2015/08/21/easy-to-read-bicycle-computer/>

[大卫·施奈德]在阳光下看不清他的自行车电脑，想要一个既可读又不需要智能手机的导航解决方案。在良好的黑客时尚中，[David] [将一个树莓 Pi 和一个 Kindle Touch](http://spectrum.ieee.org/geek-life/hands-on/build-a-readable-bicycle-computer) (带有电子墨水显示屏的那种)结合在一起。Kindle 提供了一个大而易读的显示屏。

[David]担心修改 Kindle 会违反 DCMA。结果，他不需要。他只是使用了图书阅读器的网络浏览器，并将 Pi 设置为无线接入点。一个聪明的办法是:显然，Kindle 在连接到无线网络时会尝试给亚马逊总部打电话。如果它找不到 Amazon，它会认为没有有效的网络，并将该网络视为无效。为了解决这个问题，[David]让 Pi 欺骗 Kindle，让它认为可以从 Amazon 获得有效的响应。

另一项工作是改变 Pi 上的 Python 应用程序更新屏幕的方式。[David]发现，如果没有这种优化，电子墨水显示器上的不断重绘是很烦人的。Pi 相关的硬件包括一个 GPS、一些簧片开关和一个 WiFi 加密狗。

我们很乐意将这个想法[应用到我们的摩托车](http://hackaday.com/2010/05/01/motorcycle%C2%A0computer/)上。也许是一个项目，当天气太冷骑不动的时候。

[https://www.youtube.com/embed/t4jD8E0e2ck?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/t4jD8E0e2ck?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)