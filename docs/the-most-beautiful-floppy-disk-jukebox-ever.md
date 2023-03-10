# 有史以来最漂亮的软盘点唱机

> 原文：<https://hackaday.com/2014/01/05/the-most-beautiful-floppy-disk-jukebox-ever/>

在软驱上播放音乐是一件已经被做死的事情。[kiu]的 [RumbleRail 完全是另外一回事。](http://www.schoar.de/tinkering/rumblerail/)是的，它仍然是一组播放 MIDI 文件的软盘，但工程和构建质量使它自成一类。

不同于大多数音乐软驱通常配备的电线、电源线和电路组合，[kiu]是一种精确和模块化的练习。八个软驱中的每一个都通过板载的 ATMega16 微控制器连接到它自己的驱动器。这些驱动板中的微控制器通过 I2C 总线接收来自命令板的命令。由于 RumbleRail 上的一切都是模块化的，而且事实上[kiu]使用 DIP 开关来设置每个板的 I2C 地址，这种构建理论上可以扩展到 127 个声音，或者 127 个单独的软盘驱动器，每个驱动器播放一个 MIDI 文件的一部分。

RumbleRail 还可以在独立模式下运行，不需要单独的计算机向其提供数据。MIDI 文件可以通过主控制板从 SD 卡上下载，并为软盘驱动程序解码。

如果你想构建自己的 RumbleRail，所有的电路板文件、原理图和固件都在[【kiu】的 git](https://github.com/kiu/rumblerail) 上。当然，下面有一些软盘自动点唱机的视频。

[https://www.youtube.com/embed/d6B3vYuzU4k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/d6B3vYuzU4k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/ntYL_uKkblQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ntYL_uKkblQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/pT8VArIkTpY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pT8VArIkTpY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)