# PS3 IR 加密狗适合与 Linux 机器一起使用

> 原文：<https://hackaday.com/2012/04/10/ps3-ir-dongle-tamed-for-use-with-a-linux-box/>

![](img/d0f4debed7392afdd1eb47b8aba0f71b.png "ps3_auvio")

一个男人走进一个无线电室，店员说“为什么拉长着脸？”。不，不是这样。[Ms3fgx]走进一个无线电窝棚，说“天哪，那个 PS3 IR 加密狗才两块钱”。他一直在寻找一个可以在 Linux 机器上使用的红外遥控接收器，并且[决定让这个 PS3 加密狗服从他的意志](http://www.thepowerbase.com/2012/04/use-a-cheap-ps3-ir-receiver-under-linux/)。建造最简单的红外接收器的零件要便宜得多，比如[的 FTDI 电缆版本](http://hackaday.com/2011/03/11/bitbang-ir-remote/)，或者[的基于微控制器的接收器](http://hackaday.com/2010/10/04/ir-receiver-as-usb-keyboard/)。

他插上电源，欣喜地发现它列举了。内核内置了 PlayStation 3 控制器支持，拾取这个设备没有问题。当他使用“cat”来显示输入的数据时，他得到的只是重复的垃圾。这是因为加密狗只支持索尼遥控代码。但是经过一点通用遥控器的设置，他对每个按钮都有独特的命令。难题的最后一部分是将控制器命令映射到键盘按键。这是用 QJoyPad 软件包完成的，但是有无数种方法可以重新映射这些按钮，所以用你所知道的方法吧。