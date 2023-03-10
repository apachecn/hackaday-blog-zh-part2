# 驱动 WS2811 RGB LED 像素

> 原文：<https://hackaday.com/2012/12/07/driving-a-ws2811-rgb-led-pixel/>

[Alan]一直致力于用 AVR 微控制器驱动 WS2811 LED 模块。它可能看起来像一个标准的六引脚 RGB LED，但它实际上包含一个 LED 模块和一个驱动它的微控制器。这使得它成为一个非常有趣的部分。向模块发送命令并不完全简单，因为时间必须非常精确。但是，一旦通信发生，LED 将保持相同的颜色和强度，直到你告诉它，否则。你可以把它们附在弹性条上，弹性条可以被削减到每段只有一个模块。从我们对硬件的短暂观察中，我们还没有弄清楚的一件事是每个像素是如何被寻址的。我们认为随着新值的引入，颜色值会沿着数据线逐级下降，但我们可能错了。请在评论中自由讨论。

该项目关注的是是否有可能用 16MHz AVR 芯片来驱动这些像素中的一个。它们使用 800 kHz 的单线通信，这对微控制器提出了很高的要求。他确实成功地实现了这一点，但这需要在装配时小心翼翼，以满足他的时间限制。休息后，您可以看到 led 灯在不同颜色之间淡入淡出的快速剪辑。

[https://www.youtube.com/embed/DayPkgUHU3g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DayPkgUHU3g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[ [照片来源](http://www.gree-leds.com/productshow.asp?ArticleID=V495PRYXTP)