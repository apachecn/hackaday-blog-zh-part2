# Raspberry Pi Synth 给出了一个 Softsynth 专用硬件

> 原文：<https://hackaday.com/2012/08/31/raspberry-pi-synth-gives-a-softsynth-dedicated-hardware/>

![](img/c22ffc3e807dda54dde9c2f224185bb1.png "rasynth")

对于所有的音乐家来说，[你的树莓派有一个很好的用途](http://raspberrypisynthesizer.blogspot.co.uk/2012/08/most-complex-modulation-equation-yet.html)。你期望从一个好的模拟合成器得到的所有功能都在基于 Raspberry Pi 的 polysynth 中实现了——双振荡器、lfo 和移相器——看起来在 Raspi synth 发布之前还会增加一些功能。

尽管 Raspi 合成器的“合成”部分听起来已经很棒了，但在 Rasberry Pi 上制作 MIDI 还有很多不足之处。Raspi synth 的创建者考虑过使用 GPIO 引脚作为 MIDI 接口，但是因为 GPIO 引脚不能以 31250 bps(MIDI 规范)的速度运行，Raspberry Pi 不得不浪费大部分 CPU 周期来监听 MIDI 流量。

现在，Raspberry Pi 合成器由 USB 连接的 MIDI 接口控制，正如你在休息后听到的，听起来很棒。我们迫不及待地想知道几个月后这个合成器能做什么。

[https://www.youtube.com/embed/qyU7TAi_b04?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qyU7TAi_b04?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/4YNUHoek6Zk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4YNUHoek6Zk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)