# Raspberry Pi 用于自动调光灯泡

> 原文：<https://hackaday.com/2012/12/14/raspberry-pi-used-to-automate-a-dimmable-light-bulb/>

![raspberry-pi-controlled-dimmer](img/7837b21f92111936fe9ff8ca4a1ece77.png)

[斯蒂芬]选择了安全的路线，用他的树莓调暗了一个交流灯泡。他没有在自己的出线盒内安装电源额定继电器，而是用机械连接代替电气连接。通过将伺服电机连接到调光旋钮上，RPi 可以在没有电击风险的情况下调节亮度。

他正在使用 ServoBlaster 包来驱动带有 Raspberry Pi GPIO 引脚的伺服电机。这本身很好，但他做了更多，围绕配对设计了一些不同级别的功能。黑客背后的动机是建立一个日出时钟，它在亮度方面有很大的功率。但他也利用了 RPi 的网络功能来提供基于网络的控制。它有一个滑块来设置光线水平，以及呼吸(像缓慢淡化)和闪光功能。

伺服系统在快速移动时有点噪音，但日出警报需要 30 分钟，所以齿轮实际上不会发出任何噪音。休息后在视频里看看。

[https://www.youtube.com/embed/x6sxvMdUDqw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/x6sxvMdUDqw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)