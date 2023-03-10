# 玩《我的世界》API 和树莓 PI

> 原文：<https://hackaday.com/2013/02/16/playing-with-the-minecraft-api-and-a-raspberry-pi/>

![mine](img/5c6d00fbe07534a1aca4b9088446d8f0.png)

树莓派的《我的世界》发布还不到一周，我们已经看到了一些很酷的构建，它们将我们的模拟世界与《我的世界》体素世界联系起来。[Martin]得到了《我的世界》的 Raspi 版本，并决定利用 Mojang 提供的 API 来制作一个巨大的模拟时钟,用来记录《我的世界》世界的真实时间。

基本上，[Martin]创建了一个小的 Python 脚本，在《我的世界》世界中绘制了时钟的表面和指针。《我的世界》API 附带了一些简洁的函数，比如 drawCircle 和 drawLine，所以制作一个真正的钟面就像获取系统时间和做一些 trig 一样简单。

休息之后，你可以看看[马丁]的《我的世界》时钟在行动。如果你运行的是《我的世界》的 Pi 版本，你也可以在[马丁]的 git 上用代码[让它在你的机器上运行。](https://github.com/martinohanlon/minecraft-clock)

[https://www.youtube.com/embed/ey4QpoqZLLU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ey4QpoqZLLU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)