# mono Pong:CMOS 一维 Pong

> 原文：<https://hackaday.com/2012/11/23/monopong-a-cmos-1-d-pong/>

[![](img/62bc4ff5e9e25f4e23da709941ad39c1.png "monoPong")](http://hackaday.com/?attachment_id=90503)

我们最近看到了一些一维乒乓游戏，它们都是用微控制器控制的。受到其中一些黑客的启发，[米什卡]使用少量逻辑芯片建造了[单翼](http://www.instructables.com/id/monoPong/ "monoPong")。

单簧管有四个主要部分。非稳态模式下的 555 定时器提供一个时钟源，该时钟源馈入一个 4510 十进制计数器，该计数器连接到一个 4028 BCD 转十进制解码器以驱动 led。最后，使用 4011 与非门 IC 来处理按钮按压。其中两个与非门形成一个 RS 触发器，另外两个与非门与每个玩家的按钮和位于玩家一侧的最后一个 LED 相连。如果玩家在 LED 亮起时按下按钮，RS 触发器会切换并将十进制计数器从递增计数模式更改为递减计数模式。这使得球反弹回来。

[mischka]完成了这个项目，把它放在一个木箱里，并为 led、按钮和电源开关钻孔。最终产品看起来相当不错，这是一个很好的例子，说明如何使用几个逻辑芯片来代替微控制器。

休息之后，看一个单翼的快速游戏。

[https://www.youtube.com/embed/L-oOjctCo5o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/L-oOjctCo5o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)