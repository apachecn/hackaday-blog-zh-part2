# 通过光纤的颜色复用

> 原文：<https://hackaday.com/2012/06/04/color-multiplexing-through-fiber-optics/>

![](img/895bc3a41d0eff28cae7aa292178e14e.png "RGB")

如果你想去高带宽，光纤是必经之路。从跨洋电缆到尚未出现的“光纤到户”，光纤比铜缆允许更大的带宽。在低带宽应用中，光缆使用一种颜色的光传输数据。正如 Shahriar 在试验 RGB LED 时发现的那样，有一种方法可以从光纤电缆中获得更多带宽。

在他的实验中，[Shahriar]使用了 BlinkM 可编程 RGB LED 和 [Sparkfun 颜色传感器](http://www.sparkfun.com/products/10904)。在只有一束光的光纤线路中，可以使用 PWM 同时发送多束光，但在高数据速率下，噪声会成为一个问题。使用 RGB LED，[Shahriar]发送三种级别的红色、绿色和蓝色，一次传输 9 位-非常适合在一个快速光突发中发送一个带奇偶校验的字节。

[Shahriar]的技术正是专业人员如何通过一根光缆泵送大量数据的。所有的工具、代码和 MATLAB 函数都可以在[Shahriar]的网站上找到，任何想自己尝试的人都可以使用。

在休息后的视频中，[Shahriar]分解了所有内容，包括工具、理论和实际电路。这是一个令人惊讶的视频演示，如此彻底，我们想知道[Shahriar]是否有任何教学野心。

[https://www.youtube.com/embed/A7HICe0MKB0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/A7HICe0MKB0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)