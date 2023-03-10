# 智能手机控制的 RGB 灯

> 原文：<https://hackaday.com/2012/06/08/smartphone-controlled-rgb-lamp/>

![](img/b66e6763daf8fb6b0c6aa92746519f93.png "bluetooth-controlled-rgb-lamp")

我们不断看到许多 RGB 灯，但它们的尺寸和复杂性也在不断增加。以这个再现为例，[使用了大量的 RGB LEDs，并有智能手机控制](http://www.elektroda.pl/rtvforum/viewtopic.php?p=10970239) ( [翻译](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fwww.elektroda.pl%2Frtvforum%2Fviewtopic.php%3Fp%3D10970239))。

该灯本身使用 31 个 RGB LEDs 排列成一个球体，将它们组织成三个垂直的环。它们都组合在一起(不能单独寻址)，每种颜色一个晶体管。Arduino 板负责控制，该版本包括一个蓝牙模块，用于接收命令。

正如你在上面看到的，驱动设备的 Android 应用程序真的非常好。除了用于颜色混合的滑块之外，还有一个带有颜色选择器的单独窗口。[Remick]包括最喜欢的颜色组合、颜色滚动和关闭灯的定时器等选项。我们不能在这里嵌入它，但你可以在上面的链接中找到一些演示视频。