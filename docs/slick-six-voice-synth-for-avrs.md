# 用于 AVRs 的光滑的六声音合成器

> 原文：<https://hackaday.com/2015/04/27/slick-six-voice-synth-for-avrs/>

他开始制作 AVR 合成吉他，但[Erix]最终得到了更多:一个完整的六声部 AVR 波表合成歌曲机，可以在 ATMega328 上运行——例如，在 Arduino Uno 上。

如果你是 AVR 编码器，或者对直接数字合成或 PWM 音频输出感兴趣，你应该看看他的代码( [zip 文件](http://www.erix.it/play-v6/play-v6_rev1_0.zip))。如果你只是想用芯片来制作一些曲子，看看下面的视频。

[https://www.youtube.com/embed/5My-vTky6IM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5My-vTky6IM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

在 16MHz 芯片上运行 6 个通道的 31.25 kHz 采样 8 位音频非常不错。它的底层代码通过样本更新例程中一些复杂的优化工作(如果你正在阅读的话， *play.c* 中的 *UpdateVoiceSample()* )，并通过仔细地对时间关键元素进行优先级排序。

例如，音高每两个 PWM 样本更新一次，I/O 和其他辅助播放器任务每八个样本更新一次，声音的动态音量包络每 48 个样本才重新计算一次。尽可能少地做慢算式让[Erix]掌握时机。

为了完善这些工具，[Erix]还在 Lua 中提供了 [wavetable 编辑器和歌曲生成器来编译 AVR 例程运行所需的音乐数据表。](http://www.erix.it/play-v6/tools.html)

如果你对 AVR C 编码没有印象，那么你自己也没有尝试过实现类似的东西。