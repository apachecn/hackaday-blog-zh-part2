# 迷笛的旋律营造出忧郁的氛围

> 原文：<https://hackaday.com/2014/06/12/midi-melodies-make-moody-milieu/>

![MIDI piano lights](img/ac8b4e983a1dabbcd90c758b89d60cfc.png)

在这个美丽的，记录良好的，猫辅助的黑客中，[capricorn1]通过使用键盘的 MIDI 输出来驱动爱迪生灯泡，为他令人印象深刻的钢琴技巧增加了视觉维度。

他把它们挂在一根电线导管杆上，然后把电线穿过导管连接到 DB25 连接器上。灯光由 Arduino Mega 控制，外加一个带有光耦合器的定制屏蔽，以处理过零检测。他碰巧已经有一个来自另一个项目的有 12 个 SSR 的板子。所有的电子设备都在一个重新设计的开关盒中——这些开关控制四种不同的模式:经典、速度、滚动和自动。跳转后你会在视频里看到滚动模式。

[capricorn1]使用了 Arduino MIDI 库的一个小样本，即音符开/关函数和控制改变函数来处理他的延音踏板。他列出了该项目的[完整代码](http://www.instructables.com/files/orig/FC7/0JNJ/HW8SZTBC/FC70JNJHW8SZTBC.ino)，其中包括使用 [ipMIDI 模块](http://www.nerds.de/en/ipmidi.html)通过 WiFi 实现自动化。

如果你没有 MIDI 键盘或者爱迪生灯泡，你可以做一个 [MIDI 落地钢琴](http://hackaday.com/2013/11/23/wireless-midi-floor-piano/)。不过，你需要在上面弹奏“筷子”和“全心全意”。这就像是落地钢琴的 Hello，World。

[https://player.vimeo.com/video/97796485](https://player.vimeo.com/video/97796485)