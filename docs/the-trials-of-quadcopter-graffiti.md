# 四轴飞行器涂鸦的审判

> 原文：<https://hackaday.com/2015/06/18/the-trials-of-quadcopter-graffiti/>

去年四月，涂鸦艺术家[KATSU]将一罐红色喷漆绑在一架幻影四轴飞行器上，让它飞向纽约市最大的广告牌之一，然后按下一个按钮。现在，[KATSU]，[Dan Moore]和 Adafruit 的[Becky Stern] [正试图完善一个会飞的喷漆罐](https://www.youtube.com/watch?v=aJPCvV_xGFc)，他们取得了一些成功，当然也遇到了许多失败的道具。

该团队在这个项目中使用了 Iris+,而不是今年早些时候[KATSU]使用的 Phantom，但整个努力的原理仍然是一样的:贴着墙飞起来，轻触开关，看着颜料从喷枪中喷出。为了让罐子喷漆，他们改装了一个罐子枪来接受一个微型伺服系统。这个伺服系统连接到罐头枪的触发机制，整个单位是挂在四。

让一架四轴飞行器把颜料精确地放在你想要的地方是很难的，即使是在室内。幸运的是，Iris 内部的 Pixhawk 有传感器输入和“高度保持”模式，可以接受声纳传感器，并可以编程为与墙壁保持一定的距离。这些传感器易受干扰，必须制作合适的屏蔽电缆，但传感器确实工作。

飞行的过程并不顺利。摇摆的油漆罐改变了飞行器的重心，甚至在室内飞行都很困难。不过，如果你想试一试，[Becky] [贴上他们的建造说明](https://learn.adafruit.com/quadcopter-spray-can-mod)。你可以在下面的视频中看到悬停尝试。

[https://www.youtube.com/embed/aJPCvV_xGFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aJPCvV_xGFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)