# TI 的 CC3000 WiFi 芯片获得一个库

> 原文：<https://hackaday.com/2013/06/24/tis-cc3000-wifi-chip-gets-a-library/>

大约六个月前，德州仪器发布了一款[简单、廉价的单芯片 WiFi 模块](http://hackaday.com/2013/01/12/finally-ti-is-producing-simple-cheap-wifi-modules/)。CC3000 每片 10 美元，千片订量，比 50 美元的 Arduino 以太网模块，甚至 30 美元的 Electric Imp 更好地解决了“物联网”问题。所有迹象，尤其是 TI 网站上 dev board 的频繁缺货状态，表明 CC3000 将是一款受欢迎的芯片，但直到现在我们还没有看到用于 Arduino 或其他微控制器的 CC3000 库。

[Chris] [刚刚用 Arduino 的 CC3000 WiFi 库为我们解决了这个问题](https://github.com/cmagagna/ArduinoCC3000)。他将 TI 的 MSP430 CC3000 库移植到 Arduino，即使是最基本的 Arduino Uno 也可以通过少量部件连接到 WiFi 网络。代码本身占用大约 12k 的闪存和 350 字节的 RAM，给使用 CC3000 的任何人留下足够的空间来做一些真正有趣的事情。甚至有一个精简的库，使用 2k 到 6k 的闪存，使 ATtiny 驱动的 web 服务器成为现实。

在使用带有 Arduino 的 CC3000 时有一些注意事项；这是一个 3.3 伏的部分，所以你需要一个电平转换器或一些电阻。此外，芯片在使用时消耗大约 250 毫安，所以如果你想让你的项目持续使用一整天，你需要一个结实的电池。

现在，图书馆已经不碍事了，请留意 CC3000 分线板。这里有一个，但预计很快会有更多的上市。