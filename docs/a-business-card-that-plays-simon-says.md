# 一张名片上写着西蒙

> 原文：<https://hackaday.com/2014/01/10/a-business-card-that-plays-simon-says/>

![BusinessCard_01_08](img/7ebcb8e1d4caaa1c16b6739017aac6d4.png)

当你的名字是西蒙，你想制作自己的电路板名片时，加入一个西蒙说的游戏是非常有意义的，这正是[西蒙]对他的[名片](https://sites.google.com/site/businesscardattiny45/)所做的。

你可能会看到与[工程师的紧急名片](http://hackaday.com/2013/12/02/an-engineers-emergency-business-card/)的相似之处；那是因为[西蒙]从那张卡片中获得灵感，制作了他自己的卡片。西蒙说的游戏是通过 4 个低姿态按钮和 4 个 0805 发光二极管进行的。选择运行游戏的微控制器是 ATtiny45，设置为与 Arduino IDE 一起工作。但是只有 5 个引脚可用于 I/O，[Simon]不得不放弃 4 个引脚用于 led，并将剩余的引脚配置为模拟输入。这些按钮连接到一个为模拟输入供电的分压器，因此根据按下的按钮，会读入不同的电压，因此 0 到 1023 之间的值决定了按下的按钮。

这种报道的一个伟大之处在于，它经历了使用墨粉转移法在家中蚀刻 PCB 的过程。我们不确定他愿意分发多少张刻在家里的名片，但可以肯定的是，无论谁拿到了名片，都不会忘记他的名字。

[https://www.youtube.com/embed/kEIDmOqVoGk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kEIDmOqVoGk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)