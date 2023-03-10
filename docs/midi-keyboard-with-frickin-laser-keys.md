# MIDI 键盘和该死的激光键

> 原文：<https://hackaday.com/2014/12/13/midi-keyboard-with-frickin-laser-keys/>

MIDI 乐器很酷，但它们没有激光酷。也就是说，除非你已经像[Lasse]一样[给你的 MIDI 乐器添加了激光器](http://www.instructables.com/id/Laser-Midi-Controller-Laser-Triggered-Midi-Keyboar/?ALLSTEPS "laser triggered MIDI keyboard")。

[Lasse]从一个旧的 MIDI 键盘开始。计划是回收旧键盘，而不是购买新的。在这种情况下，该团队使用了 ESi Keycontrol 49。键盘被拆开，以接触到奶油中心的电路板。[Lasse]说大多数 MIDI 键盘都带有一个 MIDI 控制板和实际的按键控制板。

一旦确定了按键控制板，[Lasse]就需要弄清楚如何在没有物理键盘的情况下实际触发按键。他通过在键盘连接到电脑时短路不同的焊盘来做到这一点。如果他按对了键盘，就会弹出一个音符。简单，但是有效。

该项目的房屋是由木头制成的。在一块上钻孔以安装 12 个激光二极管。这个数字不是任意的。熟悉乐理的人都会知道，一个八度有 12 个音符。激光器通过 USB 的 5V 电源供电。然后激光瞄准另一块木头。

在第二块被激光击中的地方钻孔。这里安装了简单的光敏电阻。每个激光传感器只需要一个电阻和一个晶体管。当激光束中断时，这个简单的分立电路足以模拟按键。不需要编程或微控制器。看看下面的演示视频，看看它是如何工作的。

[https://www.youtube.com/embed/OlU3jKbWoss?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OlU3jKbWoss?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)