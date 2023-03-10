# MIDI 中间人可以让你在混音中添加踏板

> 原文：<https://hackaday.com/2012/09/26/midi-man-in-the-middle-hack-lets-you-add-pedal-to-the-mix/>

![](img/6499348eede028469d6920aeb66db0a1.png "midi-pedal-patch")

[Sebastian]有一个朋友想在他的 MIDI 设置中使用踏板，但他的键盘不支持踏板。有些人可能会认为这是你需要买一个新键盘的信号。但是[Sebastian]已经在 MIDI 协议方面做了很多工作。他知道应该有可能[创建一个 MIDI 直通，增加对踏板](http://sebion.wordpress.com/2012/09/25/expression-pedal-midi-controllermidi-merge/)的支持。

你可以看到两根 MIDI 电缆连接到上面的盒子。一个是键盘的输入，另一个是合成器的输出。左侧还有一个用于踏板输入的插孔。内部的芯片拦截每个数据包，根据踏板输入滚动值，并将更改后的数据包传递给合成器。正如你在休息后的视频中听到的，这非常有效。

跟随[他的键盘传感器替换项目](http://hackaday.com/2012/06/05/update-many-improvements-to-optical-sensor-based-piano/)，捕捉更多【Sebastian】的 midi 作品。

[https://www.youtube.com/embed/w5sfG_973kQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/w5sfG_973kQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)