# 把玩具钢琴变成 MIDI 键盘

> 原文：<https://hackaday.com/2012/11/28/turning-toy-pianos-into-midi-keyboards/>

![](img/e7cfa3f45eed5d718a48977d1da15e48.png "MIDI")

制作 MIDI 设备总是一个伟大的微控制器项目，几乎每个人都有一个旧的玩具键盘放在壁橱后面或地下室里。[JenShen]决定用这些玩具键盘中的一个[做一个 MIDI 键盘](http://www.codetinkerhack.com/2012/11/how-to-turn-piano-toy-into-midi.html)。

使用的键盘[JenShen]是一个简单的内置语音的卡西欧键盘。在撕开键盘的内脏后，唯一剩下的就是按键下面的一排按钮。这些按钮排列成行/列矩阵，因此[JenShen]需要解码这个矩阵，然后将结果发送到 Arduino 进行处理。

74HN595 移位寄存器用于读取按键下的 8 行按钮，同时这些行被绑定到“duino”上的不同输入引脚。这使得[JenShen]可以用 Arduino 扫描键盘矩阵，生成 MIDI 音符并发送给其他合成器。

在休息后的视频中，你可以查看[JenShen]的电路和代码，这些电路和代码允许他将一个玩具键盘变成一个合适的 32 音符 MIDI 键盘。它对速度并不敏感，但他说他会在以后的文章中向大家展示如何实现这一点。

[https://www.youtube.com/embed/AEqzr5NUdQo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AEqzr5NUdQo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)