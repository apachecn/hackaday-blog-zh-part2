# 由 TI-84+控制的四轴飞行器

> 原文：<https://hackaday.com/2012/08/15/toorcamp-quadcopter-controlled-by-a-ti-84/>

[![](img/e42b06d2e72ea8582e8791e04ce9b7f0.png "Blue TILP")](http://hackaday.com/?attachment_id=82688)

当您将 TI-84+图形计算器与附加的蓝牙模块、1 瓦 Alfa wifi 加密狗和 Parrot Wifi 四轴飞行器结合在一起时，会发生什么？你得到了一个远程四轴飞行器，它由 TI-84+方向板控制。

这个 TI-84+看起来像一个标准的问题学校计算器，但是[ [欧文](http://hackniac.com/ "Owen") ] [增加了一个 ATTiny13 微控制器](http://www.hackniac.com/blog/?p=1139 "Blue TILP")和一个蓝牙模块，它可以嗅探计算器的 I/O 端口。这允许与笔记本电脑进行双向通信。他在笔记本电脑上编写了几个 Python 脚本，从计算器接收数据，并向 Parrot 四轴飞行器发送命令。高功率 wifi 模块允许四轴飞行器有相当好的范围，它飞过 Toorcamp 场地。

当然，拥有一个带有无线通信的看起来很简单的计算器还有其他一些用途。数据可以通过蓝牙从手机显示在计算器上。用计算器访问维基百科或者 WolframAlpha 怎么样？尽管有这种可能性，[欧文]确实说过他从来没有用它来作弊。