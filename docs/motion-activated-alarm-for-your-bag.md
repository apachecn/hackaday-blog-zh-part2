# 你的包的运动启动警报

> 原文：<https://hackaday.com/2015/01/27/motion-activated-alarm-for-your-bag/>

我们很多人都随身带着一个装有昂贵个人物品的包。不过，整天带着一个包可能会很痛苦。如果你想把它放下一段时间，你经常要设法盯着它，以确保没有人偷它。[Micamelnyk]决定以[运动感应报警器](http://hackaday.io/project/3573-trinketpro-movement-alarm-for-bag-theft-prevention "Motion sensing alarm")的形式来解决这个问题。

该设备是围绕一个小饰品 Pro 构建的。Trinket Pro 是 ATMega328 的一种分线板。它与 Arduino IDE 兼容，还包含一个 USB 端口，便于编程。这个小饰品被连接到一个 GY-521 加速计上，这使它能够检测运动。当饰品感觉到设备被移动时，它会从压电扬声器发出响亮的高音哀鸣声。

要启动设备，用户首先按住电源按钮 3 秒钟。然后用户有十秒钟的时间输入他们的密码。这可确保设备不会意外启动，并且用户在启动设备之前始终记得密码。代码通过安装在印刷电路板上的四个按钮输入。代码和代码长度都可以在 Trinket 软件中轻松修改。

输入代码后，状态 LED 将稳定亮起。这向用户表明该设备必须静止放置。LED 将在 20 秒后熄灭，表示警报现在已启动。如果行李一次移动超过五秒钟，警报就会响起。轻微的延迟给用户足够的时间解除警报。该参数也可以通过软件轻松配置。