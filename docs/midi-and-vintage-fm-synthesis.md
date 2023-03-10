# MIDI 和复古 FM 合成

> 原文：<https://hackaday.com/2014/07/08/midi-and-vintage-fm-synthesis/>

![FM](img/b0b09c620bbcf6a8fc7236bbc30df8de.png)

在计算机可以播放和录制远远超过 CD 质量的音频之前，声卡非常非常酷。大多数 80 年代的音频芯片，来自 Commodore SID，几乎是芯片上的合成器，但你也可以在古老的 ISA 声卡中找到类似的设置。[埃米利奥]抽出其中一张卡，上面有一个阿德利·OPL2 芯片，[并用一个 PIC micro 创建了他自己的 FM 合成合成器](http://ficara.altervista.org/?p=1381)(它，[translator on](https://translate.google.com/translate?sl=it&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fficara.altervista.org%2F%3Fp%3D1381&edit-text=&act=url)，尽管谷歌正在搞砸格式)。

雅马哈 YM3812 芯片，也称为 OPL2，是一个非常小的封装中相当完整的合成器，使用 FM 合成一些非常独特的声音。一旦[埃米利奥]让 PIC 向声音芯片发送命令，他就添加了 MIDI 支持，使他能够用键盘而不是跟踪器来演奏这种老式的“片上合成器”。

从下面的视频来看，这听起来很棒，这是[Emilio]为一个简单的演示而进行的混音。

[http://www.dailymotion.com/embed/video/x212fa8](http://www.dailymotion.com/embed/video/x212fa8)