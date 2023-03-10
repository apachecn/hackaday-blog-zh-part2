# 作为 MIDI 乐器被遗忘的摇滚乐队鼓控制器

> 原文：<https://hackaday.com/2015/07/18/forgotten-rock-band-drum-controller-as-a-midi-instrument/>

碰巧有一个旧的摇滚乐队鼓控制器在你的客厅里收集灰尘？如果你还有一个备用的 Arduino，并且不介意扔掉那个塑料的大学纪念品，那么你已经得到了大部分有可能成为你新的打击乐器 MIDI 的东西。在他的项目视频中,[Evan Kale]概述了将这种不受欢迎的塑料变成一种有能力的录音工具的必要步骤。

[埃文]描述的整个过程不到 7 分钟。对于我们这些刚刚开始使用 MIDI 的人来说，这看起来是一个很好的周末努力。打开吉他英雄架子鼓控制器的背面后，内部的主板可以很容易地更换为标准尺寸的 Ardunio(与目前的安装孔完全匹配)。视频开始大约 4:50 时[Evan]解释了如何在 Arduino 上添加一个基本的 perf-board 屏蔽，将每个鼓垫中的压电传感器连接到微控制器的模拟引脚。当连接到 Arduino 的串行输出引脚时，套件背面内置的 MIDI 插孔也可以作为 MIDI 输出重复使用。通过调整【Evan 的】[示例代码](https://github.com/evankale/ArduinoMidiDrums)，您可以拨入仪器的反馈，以匹配每次击打的强度。

视频与所有的细节是在跳跃之后。或者你可以试试 MIDI hack 的另一种方式，使用一套[鼓作为吉他英雄或摇滚乐队的控制器，而不是](http://hackaday.com/2008/11/30/midi-drums-for-guitar-hero-and-rock-band/) …

[https://www.youtube.com/embed/vi-w_WqJjzQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vi-w_WqJjzQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)