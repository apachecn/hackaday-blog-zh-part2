# 将红外遥控器与 Arduino 配合使用

> 原文：<https://hackaday.com/2012/07/23/using-an-ir-remote-with-your-arduino/>

![](img/b040d6f2c8cbc748e8de7b260a9e9ed0.png "Remote")

如果你曾经需要一个短程遥控器来完成一个项目，[firestorm]可以帮你解决这个问题。他发布了一个很棒的教程[,教你使用红外遥控器](http://www.yourwarrantyisvoid.com/2012/07/10/hardware-remote-control-your-arduino/)在每个人都喜欢的微控制器平台上做任何事情。

[firestorm]使用 Arduino 远程库来解码他遥控器上的按键。上传库中的红外接收演示后，Arduino 吐出了红外接收器所看到的十六进制代码。[firestorm]写下了这些，并能够对他的 Arduino 进行编程，以响应每个单独的按钮按压。

在弄清楚他的遥控器的红外代码后，[火焰风暴]把一个移位寄存器扔进他的面包板，并附上一个七段 LED。因为[firestorm]知道遥控器上数字按钮的代码，所以当按下遥控器上相应的按钮时，很容易让 LED 显示屏闪烁一个数字。

一个单独的七段显示器可能不是非常有用，但是通过[firestorm]的教程，很容易用一个简单的红外接收器为您的 Arduino 提供一些远程控制功能。对于几块钱的零件来说还不错。