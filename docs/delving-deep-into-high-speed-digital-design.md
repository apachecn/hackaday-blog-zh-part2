# 深入研究高速数字设计

> 原文：<https://hackaday.com/2014/06/21/delving-deep-into-high-speed-digital-design/>

![scope capture showing ringing affect in a high speed digital signal](img/9f0636e1cbc1c23be2d340ba58334003.png)

在高速数字电路中，快并不一定意味着“高时钟速率”。[Jack Ganssle]出色地解释了高速数字电路中信号的转换时间与信号本身的速度一样重要。当转换时间很长时，大约 20 纳秒，一切都很好。但是当你把它缩短到只有几纳秒时，事情就变了。通常，阻抗不匹配会导致振铃效应。

当信号从驱动器沿走线传播并到达接收器时，如果阻抗(即含有频率成分的电阻)不完全匹配，部分信号将反射回驱动器。然后，反射信号返回驱动器，阻抗不匹配将导致另一次反射。它来回移动，产生你在示波器上看到的“铃声”。

[Jack Ganssle]继续解释简单的电阻网络如何有助于匹配阻抗，以及如何在具有快速转换时间的电路中使用这些电阻网络，尤其是在使用示波器读取读数的情况下。因为示波器探头本身会引入阻抗并导致振铃。

如果你没注意到的话，[杰克·甘斯勒]碰巧也是黑客日奖的评委之一。

[https://www.youtube.com/embed/MJpDFnRQw8s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MJpDFnRQw8s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)