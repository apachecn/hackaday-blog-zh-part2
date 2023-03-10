# 少年变成了 MPC

> 原文：<https://hackaday.com/2014/10/04/the-teensy-becomes-an-mpc/>

如今，Akai MPC 是每个录音室的主要设备，它在 90 年代初只是一个简单的采样槽盒。一些可分配给不同样本的力敏垫的形状因素，对于稍微有点 MIDI 设备的人来说应该是熟悉的，但这些很少是定制的设备。现在，它运行在一个小小的上。[Michele]用 Teensy 3.0、Teensy 音频适配器板和使用替换 MPC 板的巧妙 PCB 设计创建了自己的 MPC 风格 MIDI 板控制器。

[Michele]的 MPC 第一次出现在 MIDI hacklet 中的[,但当时唯一的工作组件是 pads 本身。速度敏感垫由铺设在单个醋酸纤维板上的两条铜走线构成。一点](http://hackaday.com/2014/07/11/the-hacklet-7-midi/) [Velostat](http://en.wikipedia.org/wiki/Velostat) 粘在垫的背面，所以当垫被按压时，它接触两条迹线。焊盘被压得越重，阻抗越低，所有的东西都被送到一个模拟引脚，每个焊盘都变成了一个力敏电阻。

解决了 MPC 的关键特性后，[Michele]将注意力转向了设备的采样和软件。新的 Teensy 3.0 音频适配板——[和一个伟大的新库](http://hackaday.com/2014/09/30/the-teensy-audio-library/)——照顾一切。[Michele]他的 MPC 还没有一个合适的视频，但他昨天在罗马 Maker Faire 上拍摄了一个随机的家伙玩他的机器。你可以看看下面。

[https://www.youtube.com/embed/8R2ZX7gavcU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8R2ZX7gavcU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)