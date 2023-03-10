# 为策略游戏构建小键盘

> 原文：<https://hackaday.com/2013/09/10/building-a-small-keypad-for-strategy-games/>

[![](img/69bcb95facb05de91cb674439f94e240.png)](http://hackaday.com/wp-content/uploads/2013/09/dsc04002.jpg)

一个月前[安德烈亚斯]又开始玩星际争霸 2 了。由于他不习惯普通键盘上的默认热键，[Andreas]决定[打造自己的](http://chaozlabs.blogspot.de/2013/09/keypad.html)。

他首先从他放在周围的旧键盘上回收按键，然后 3D 打印出你在上图中看到的外壳，以适应它们。键盘电气设计是一个简单的矩阵，似乎他自己蚀刻的 PCB。为了提供所需的 USB 连接，选择了 Atmega8U2。它配有一个预编程的 USB 引导程序，当系统启动时按下左键，[Andreas]选择激活它。HID 类是使用 LUFA-USB 框架实现的，最终产品看起来绝对不错。

复制他的设计所需的所有文件都可以在这里找到。你还可以查看[另一个星际争霸键盘](http://hackaday.com/2013/07/05/a-custom-starcraft-keyboard/)和[一个我们之前展示过的人体工程学键盘](http://hackaday.com/2013/05/28/one-mans-adventures-in-custom-keyboard-development/)。