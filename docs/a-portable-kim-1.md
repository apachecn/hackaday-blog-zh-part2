# 便携式 KIM-1

> 原文：<https://hackaday.com/2015/01/20/a-portable-kim-1/>

KIM-1 是第一台使用 6502 的计算机，这种 CPU 后来出现在苹果、Ataris、Commodores 和任天堂娱乐系统中。作为第一个的*，KIM-1 实际上只用 1k 的 ROM 和 1k 多一点的 RAM 做不了很多事情。这对任何拥有 Arduino 的人来说都是一个好消息；你可以用一个键盘和 7 段显示器轻松复制整个 KIM-1。[【斯科特】就是这么做的](http://geodesicsphere.blogspot.com/2015/01/kim-uno.html)，他把它放在一个外壳里，看起来就像 70 年代末工程实验室里的家一样。*

这一建造的动力是[斯科特]发现了 KIM-Uno，这是一个使用 Arduino Pro Mini 的 KIM-1 的套件克隆体。工具包应该在几周内到达，所以在那之前，他决定看看是否可以用他闲置的零件拼凑一个。

在一个手持工业外壳内是一个 Arduino Uno，有一个 protoshield 连接键盘和显示器。这个显示器是一个 11 位的七段显示器[Scott]从一家旧货商店买的，金属圆顶键盘来自一个 hamfest。

让软件工作起来需要一些工作，但最重要的部分只是对标准 Arduino 库的修改。

现在[斯科特]有了一个 KIM-1 的复制品，他可以对这个虚拟的 6502 进行编程，一次一个十六进制数字，运行微棋，或者把整个东西[当作一个可编程计算器](http://obsolescence.wix.com/obsolescence#!kim-uno-calculator/cgru)。