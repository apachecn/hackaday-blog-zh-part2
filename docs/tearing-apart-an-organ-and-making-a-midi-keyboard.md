# 拆开一个风琴，做一个 MIDI 键盘

> 原文：<https://hackaday.com/2013/06/25/tearing-apart-an-organ-and-making-a-midi-keyboard/>

![pedul](img/28a28615d2ebf5c8da39c00c38e3bcd7.png)

如果你在一个乐队里，身边放着一个旧的、死了的器官，你会怎么做？[当然是造一个 MIDI 脚控器](http://zaardvark.blogspot.co.uk/2013/06/zaarduino-midi-organ-pedals.html)。

分发完旧的器官内脏后，[马克]把踏板装在一个漂亮的旅行箱里，开始研究电子设备。他的第一个爱好是在一块条板上安装 Arduino Pro Mini，但在那之后，他决定学习 Eagle 并制作 PCB。风琴踏板的每个键都连接到一个由 Arduino 读取的开关，Arduino 通过 MIDI 将数据发送到 Korg 微型采样器。

管风琴的膨胀踏板也被重新使用，但因为踏板上的旧白炽灯已被烤焦，所以被 LED 取代。它仍然工作，允许[马克]在他的新的，花哨的，MIDI 脚控制器上做音量膨胀。

你可以看看下面这个控制器的视频。

[https://www.youtube.com/embed/ehf451c4AAk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ehf451c4AAk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)