# 动画 LED 情人节心

> 原文：<https://hackaday.com/2015/02/13/animated-led-valentine-heart/>

离情人节只有一周了，[亨利]需要快速思考。他想为他的女朋友做点什么，但由于时间有限，他需要利用现有资源。在搜罗了一些零件和一些 CAD 工作后，他完成了一个漂亮的 LED 情人节心形动画。

[Henry]有一堆旧项目遗留下来的 led 灯。这些表面贴装 LED 非常酷。它们外形小巧，在一个封装中集成了红色、绿色和蓝色 led。最重要的是，他们有一个内置的控制电路，使每个 LED 单独寻址。它类似于我们过去见过的 [LED 灯条](http://hackaday.com/2009/06/17/addressable-rgb-led-strip/ "LED Strips")，只是现在控制电路内置在 LED 中。

从发光二极管开始，[亨利]决定建造一个大的动画心脏。作为一个注重细节的人，他从三个同心心形开始设计，设计出了完美的 LED 摆放方式。这些心在 Excel 中绘制出来，然后进行缩放，直到他最终得到他喜欢的东西。这个最终设计显示了每个 LED 的放置位置。

下一步是在 Altium Designer 中设计 PCB。[Henry 的]设计是双面的，两侧都有大的铜平面。他选择很好地利用额外的铜表面，在背面蚀刻一个定制的设计，上面有他女朋友的名字。他为运行动画的 ATMega48 芯片留出了空间。最后，他把设计送到一家工厂，并设法在 48 小时后取回。

将所有组件焊接到位后，[Henry]为 led 编写了一些动画。他还建造了一个定制的框架来容纳 PCB。该框架包括一个白色屏幕，可以漫射和柔和 led 发出的光。最终产品看起来很棒，一定会赢得任何极客的心。

[https://www.youtube.com/embed/9jf7k3OPVIw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9jf7k3OPVIw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)