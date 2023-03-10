# 使用 Teensy 播放音乐与您的绘画

> 原文：<https://hackaday.com/2015/02/21/play-music-with-your-painting-using-teensy/>

[索菲亚·布鲁克纳]和[埃里克·罗森鲍姆]合作的[sab-art]创造了[一幅触摸感应音乐画](http://www.instructables.com/id/Touch-Sensitive-Musical-Painting/)。最初，基本的丙烯颜料被用于画布的大部分。一旦干燥，导电涂料被用来制作将用于电容式触摸感应的形状。作为增加坚固性的一个额外步骤，钉子被钉在每个画的形状上，并与画后面的电线连接。这些电线然后连接到一个 [Teensy++ 2.0、](https://github.com/ericrosenbaum/makeymakey-midi/blob/master/makey_teensy_midi.ino)的输入，使用基于 [MaKey MaKey](hackaday.com/2012/11/22/dead-nes-controller-used-as-a-makey-makey-shield/) 的 Arduino 代码输出 MIDI。MIDI 然后被发送到 Mac Mini，Mac Mini 然后使用 Ableton Live 合成声音。不过，任何 MIDI 处理软件都可以。对于这幅特定的画，使用了外部扬声器，但是将扬声器结合到您自己的作品中当然是可能的。

这个项目的一个好的方面是，它可以像你选择的那样简单或复杂。多个导电形状可以通过背面连接到同一个微小的输入端，这样它们就可以发出相同的声音。虽然[sab-art]看起来更抽象，但它可以用于任何风格。想象一下，画一幅[狗玩扑克](http://en.wikipedia.org/wiki/Dogs_Playing_Poker)的画，当你触摸它时，每只狗都以各自品种的方式吠叫，或者让宇宙飞船发出“皮尤皮尤”的声音。对于一个真正的元时刻，一个 MIDI 键盘的交互式 MIDI 绘画将是崇高的。[sab-art]正在对每一幅新画的制作过程进行改进，因此更多富有想象力的音乐艺术作品即将面世。我们迫不及待地想看到和听到他们！

[https://player.vimeo.com/video/74969550](https://player.vimeo.com/video/74969550)

[通过指令]