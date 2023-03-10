# 带有机载合成器的电子木管乐器

> 原文：<https://hackaday.com/2015/06/20/an-electronic-woodwind-with-an-onboard-synthesizer/>

大约一年前，我们在 Hackaday.io 上看到一个 MIDI 风控制器的项目。键盘 MIDI 控制器多如牛毛，但如果你想要听起来像铜管或木管乐器的东西，你需要由呼吸传感器控制的东西。从那以后，[这个项目已经更新了一个机载合成器](https://hackaday.io/project/2992-hopkins-electronic-aerophone/log/19547-onboard-synthesizer-demonstration)。这听起来很棒，由于一些有趣的组件，零件数量实际上非常低。

这个项目使用的合成器只是一个单芯片——[【Jan ost man】](https://janostman.wordpress.com/category/dsp-g1/)的 DSP-G1。这不是一个定制的 ASIC 或任何花哨的东西；它只是一个 DIP 格式的 8 引脚 ARM 微控制器，即 LPC810。

仪器的其余部分只是沿着身体的一系列压力传感器和一个呼吸传感器。该计划是将所有的电子设备——读取触摸和呼吸传感器的微控制器、DSP-G1 芯片和电池——都放在仪器的主体内。这将是非常酷的东西，比今天可用的风力控制器更有能力。

下面可以看到几个风控器的视频。

[https://www.youtube.com/embed/e7Gd0bjZoBo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/e7Gd0bjZoBo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/HFZy-M_Pnf4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HFZy-M_Pnf4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/SlMxqbnq5lY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SlMxqbnq5lY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)