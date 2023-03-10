# 电路弯曲玩具键盘是 MIDI 控制的

> 原文：<https://hackaday.com/2013/10/11/circuit-bent-toy-keyboard-is-midi-controlled/>

![tymkrsKeyboard](img/337c59e02a9cbb49ab76be7604babca6.png)
【tym krs】剧组想出了一个相当巧妙的[电路弯曲玩具键盘破解](http://www.youtube.com/watch?v=-D22AWj1go0)。自从我们看到一个好的[电路弯曲黑客已经有一段时间了。](http://hackaday.com/2011/01/11/intro-to-circuit-bending/)这个项目最初是为了演示[tym krs]“MIDI In Me”套件。一个廉价的玩具键盘因其发声板而被牺牲。像许多廉价的大规模生产的玩具一样，这种板基于 COB(板上芯片)封装。主 ASIC 的硅芯片直接放置在 PCB 上，并焊接到焊盘上。圆形环氧树脂滴保护一切。

[Tymkrs]发现他们的键盘中有许多芯片垫没有被使用。这些输入似乎触发了鼓，可能用于不同的玩具。这些输入，再加上“demo song”按钮，就成了这次黑客攻击的基础。MIDI 输入被发送到一个[视差推进器](http://hackaday.com/2011/01/04/getting-started-with-the-parallax-propeller/)。该道具运行一个程序，该程序将根据 MIDI 音符开/关命令设置其 I/O 引脚。然后，I/O 引脚驱动晶体管，将信号注入键盘的按钮输入。

[Tymkrs]甚至在键盘的主时钟电路上使用了分压器。改变主时钟会导致一种弯音效果，这种效果在弯音玩具中很常见。与按钮一样，MIDI 信号命令道具启用或停用振荡器信号注入。电位计用于调整振荡器频率。

这一切的美妙之处在于，整个破解过程可以通过运行在 PC 上的 MIDI 音序器来控制。发送快速音符开/关命令会产生一些有趣的效果。
视频的后半部分是结果的即兴表演。虽然我们不会把它放在 mp3 播放器上，但它肯定比我们最近听的大多数沃贡诗歌要好。

[https://www.youtube.com/embed/-D22AWj1go0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-D22AWj1go0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【谢谢兰迪！]