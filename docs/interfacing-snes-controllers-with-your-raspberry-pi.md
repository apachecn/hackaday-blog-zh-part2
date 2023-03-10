# 将 SNES 控制器与您的树莓 Pi 接口

> 原文：<https://hackaday.com/2012/07/05/interfacing-snes-controllers-with-your-raspberry-pi/>

![](img/3cf5330764417a3c356bf8764d051c9b.png "snes-ports-for-rpi")

这套可爱的电线让[Florian] [将股票超级任天堂控制器连接到他的树莓 Pi](http://petrockblog.wordpress.com/2012/07/03/snesdev-rpi-a-snes-adapter-for-the-raspberry-pi/) 。左上角的 IDC 连接器插入 RPi 上的 GPIO 头，而不是使用中间 USB 转换器走[的路线。](http://hackaday.com/2011/11/30/funtendo-connects-all-your-nintendo-controllers-to-a-pc/)

这个设置可以让你一次连接两个控制器，所以你可以在休息后的剪辑中看到马里奥赛车。端口本身是从一对 SNES 延长线上拔下来的。由于按钮信号是通过移位寄存器推送到控制台的，因此每一个只需要五根线(电压、接地、数据、时钟和锁存)。据我们所知，Raspberry Pi 引脚不支持 5V 电压，因此如果您自己构建该电路，可能需要增加一些电平转换。

[Florian]写了一个 C 程序，它将来自控制器的数据转换成 HID 键盘输入。这应该使它在模拟器设置方面非常灵活，并且将该技术用于不同风格的控制器也应该非常容易。

[https://www.youtube.com/embed/4TvH1ohcCus?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4TvH1ohcCus?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)