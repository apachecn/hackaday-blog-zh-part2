# 家酿吉他调谐器也包括 MIDI 输出

> 原文：<https://hackaday.com/2012/10/27/homebrew-guitar-tuner-also-includes-midi-out/>

几年前，[弗雷德里克]的姐夫想要一个吉他调音师作为圣诞礼物。【frédéric】[没有出去买一个，而是拿出烙铁，从头做了一个](http://deambulatorymatrix.blogspot.ca/2010/11/digital-chromatic-guitar-tuner-2008.html)。

[Frédéric]的调谐器是围绕一个 ATMega168 uC 在一个带有 LM386 放大器的真正的裸机板上构建的。显示器是一个标准的 20×2 LCD 字符显示器，界面是从踏脚转盘示意图的页面上撕下来的，带有一个非常沉重的脚踏开关。

检测[弗雷德里克]调音器中播放的音符的频率涉及到相当多的数学知识。为了测量频率，Arduino 对来自输入插孔的波形进行采样。该信号被延迟几分之一秒，然后测量真实波形和延迟波形下方的面积。该延迟在原始波形上滑动，直到真实样本和延迟样本之间的区域最小。在这一点上，延迟波形将正好比真实信号晚一个周期，并且可以计算每秒的周期数。它叫做尹算法，你可以[在这里](http://recherche.ircam.fr/equipes/pcm/cheveign/pss/2002_JASA_YIN.pdf)了解更多。

由于[Frédéric]已经知道调谐器中播放的确切频率，他认为给 MIDI 转换器添加一个小型模拟音频并不重要。这项功能(如休息后的视频所示)将吉他的声音转换为 MIDI 音符。这是单声道的，可能有点多余，但仍然非常酷。

[https://www.youtube.com/embed/oGKE1vmAWCA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oGKE1vmAWCA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)