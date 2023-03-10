# 支持 Wi-Fi 的车库门开门器

> 原文：<https://hackaday.com/2013/09/26/wi-fi-enabled-garage-door-opener/>

通常情况下，互联网控制的家用设备是由各种部件拼凑而成的。这对于一个原型来说是很棒的，但是如果你正在寻找一个可以在你的车库里使用十年的东西，你将需要一个稍微干净和更坚固的东西。[Phil]的[互联网车库门开启器](http://www.megunolink.com/garage-door-opener/)就是这样，里面装满了为他的 Arduino 供电系统定制的外壳。

[Phil]建造的主要硬件是一个 [Freetronix EtherTen](http://www.freetronics.com/products/etherten#.UkRCgcakpP8) ，一个带有内置以太网接口的 Arduino 克隆体。除此之外，电子设备很简单:一个继电器，晶体管和二极管提供了从以太网到车库开门器的连接。

该设置的软件包括一个设置网页的主文件、串行监视器和主程序循环。有一堆初始化网页、向 EEPROM 写入密码、激活门以及设置 MAC 和 IP 地址的类。

用这个遥控器开门很容易:使用任何支持 WiFi 的智能手机或平板电脑，[Phil]只需登录他的网络，浏览 Arduino 上托管的页面，然后输入密码。从那里，打开门只是按下一个按钮。可以使用 [MegunoLink](http://www.megunolink.com/) 输入密码和其他配置设置。该软件还包括一个串行监视器来记录谁在何时打开了门。

这是一个有趣而紧凑的系统，启动方便。你可能有时会忘记你的车库门开启器，但我们认为如果你发现自己没有手机，关闭的车库门是你最少的问题。