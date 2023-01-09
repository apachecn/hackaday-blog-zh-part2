# 右手失去工作，因为头鼠进入捕鼠场

> 原文：<https://hackaday.com/2014/12/20/right-hand-loses-job-as-head-mouse-enters-mousing-arena/>

在你的电脑屏幕上移动光标是每天都会发生的事情，我们人类对此并不太在意。但是如果你不再需要将手从键盘上移开会怎么样呢？当然，也有带跟踪点甚至跟踪板的键盘离按键不太远，这并不太糟糕。如果你可以把脸稍微指向鼠标移动的方向，会怎么样？[Sci-Spot]的人想知道同样的问题，并提出了一个 DIY 头鼠。

这个概念非常简单；一个网络摄像头安装在用户的头上，指向电脑屏幕。安装在屏幕顶部的是一个红外 LED。我们的眼睛看不到红外光，所以它不会令人讨厌或分心。然而，通过在镜头上放置几层相机底片，相机被过滤成只能看到红外。在你抱怨把相机绑在你的头上之前，只要想想把它放在帽子里，我们已经看到它被用于自适应技术[像 PS3 控制器](http://hackaday.com/2013/07/05/playstation-3-contolled-with-head-movement/)。

编写定制软件来移动鼠标光标；看到上面对话框的黑色窗口了吗？这代表网络摄像头的视野，白点是红外 LED。当用户的头部移动时，红外 LED 会根据相机的视野移动，进而告诉计算机将光标移动一定的距离。有几个选项可用，如“放大”和“死区”,前者可以在头部移动一定量的情况下改变光标的移动量，后者可以忽略呼吸导致的极小移动。

没有提到按钮点击是如何被记录的，但是我们认为在空格键下面有几个按钮会很棒。控制软件可以在 Sci-Spot 网页上下载，供那些想自己制作的人使用。