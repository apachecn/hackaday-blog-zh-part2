# 单宁 DIY MIDI 控制器

> 原文：<https://hackaday.com/2014/03/08/the-tannin-diy-midi-controller/>

![tannin-ctlr](img/1f8d4c93df358c4ac73f3f4bad59a2ec.png)

[Shantea]需要一个 DJ 控制器。虽然有商业控制器，但没有一个符合他的要求。他通过[构建丹宁 DIY MIDI 控制器](http://projects.hackaday.com/project/62-Tannin-MIDI-controller)解决了这个问题。Tannin 有 19 个按钮、16 个电位计和 4 个发光二极管。短按和长按按钮可以发送不同的 [MIDI](http://en.wikipedia.org/wiki/Midi) 信息。Pots 可以发送 6 个音符开/关信息以及 MIDI 控制信息，具体取决于它们的位置。led 随着 MIDI 输入时钟的节拍闪烁。一切都是可编程的，可以用成千上万种不同的方式映射。该系统的核心是 Arduino Nano。[Shantea]使用[无毛 midi](http://projectgus.github.io/hairless-midiserial/) 库将 midi 转换为串行。Arduino 通过 USB 串行接口与 PC 连接。在主机端，他运行 [loopbe30](http://www.nerds.de/en/loopbe30.html) 来创建一条虚拟 MIDI 电缆，连接到他的 DJ 软件 [Traktor](http://www.native-instruments.com/en/traktor/) 。

我们喜欢内在和外在看起来一样好的建筑，单宁在这方面给人留下深刻印象。框架是中密度纤维板，控制面板是在 3 毫米的有机玻璃上激光蚀刻的塑料。我们真的很喜欢单宁的黄酮。在盒子里，电线通过拉链和纽扣网格下面的木条保持整齐有序。[Shantea]在将花盆连接到飞线时遇到了一些噪声问题，因此他使用了一个带有接地层的定制印刷电路板，将花盆分成两组，每组 8 个。这个结果是任何一个[控制者](http://en.wikipedia.org/wiki/Controllerism)都会感到骄傲的。点击休息时间，查看丹宁的作用。

[https://www.youtube.com/embed/zh2d0BJjfGw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zh2d0BJjfGw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)