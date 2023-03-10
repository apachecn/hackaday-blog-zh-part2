# 带数字卡尺的三轴位置指示器

> 原文：<https://hackaday.com/2014/01/19/three-axis-position-indicator-with-digital-calipers/>

[![](img/03fe13c3edb551603a0aa4355f40c746.png)](http://hackaday.com/wp-content/uploads/2014/01/img_5149_sc.jpg)

[Malte]刚刚为他的 Wabeco F1200 铣床完成了一个小项目:一个用于三个数字滑动卡尺 ( [译自德语](http://translate.google.com/translate?js=n&sl=auto&tl=en&u=www.mtahlers.de/index.php/diverses/messschieberanzeige))的[紧凑型外部显示器。你可能已经猜到了，[Malte]非常幸运，能够将拆卸的卡钳安装到机器上，并使用它们进行定位。在开始这次冒险之前，他注意到互联网上也有类似的项目，但是所有使用的卡尺都有不同的数据接口和协议。[Malte]买的卡钳有一个迷你 USB 连接器，尽管接口本身不是 USB。由于在该接口上找不到任何信息，他转向示波器来解码协议。](http://www.mtahlers.de/index.php/diverses/messschieberanzeige)

[Malte]然后建立了一个基于 AVR 的平台，它可以读出三个卡钳，并在上面显示的点阵 LCD 上显示位置数据。AVR 固件是用 Basic 和汇编语言混合编写的。源代码、原理图和其他资源可以从项目的网页上下载。我们对最终结果的专业方面印象深刻。

[https://www.youtube.com/embed/iRqhlThrwV4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iRqhlThrwV4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)