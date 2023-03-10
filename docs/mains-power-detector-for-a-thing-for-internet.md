# 物联网电源检测器

> 原文：<https://hackaday.com/2014/07/06/mains-power-detector-for-a-thing-for-internet/>

![inductor](img/bfbe6143d781e97e40abb9797bbb9fd6.png)物联网正在快速到来，虽然没有人能告诉我们*到底是什么*，但我们知道它与控制电器和灯或其他东西有关。能够控制一些东西固然很好，但是能够辨别一个有电源连接的电器是否打开也同样有价值。[谢恩] [有一个非常简单的电路](http://www.wattnotions.com/mains-power-detection-circuit/)他一直在努力做到这一点:判断连接到电源的东西是否打开，并通过无线链路传递信息。

[Shane]的电路有两个基本部分——一个 RLC 电路检测流经导线的电流，然后将该电路馈入由三个运算放大器构成的仪表放大器。其输出经过一个二极管，直接到达微控制器的 ADC，准备好传输到你的本地 thingnet 将拥有的任何无线电设置。

这是一个非常简单的电路，可能用你在元件抽屉里能找到的不到一美元的元件就能制造出来。[Shane]有一个连接到微控制器的电路演示，您可以在下面查看。

[https://www.youtube.com/embed/ef1Ce731i0M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ef1Ce731i0M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)