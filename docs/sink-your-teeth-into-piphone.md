# 咬紧牙关

> 原文：<https://hackaday.com/2014/04/26/sink-your-teeth-into-piphone/>

你曾经梦想过从智能手机膨胀软件中独立出来吗？如果你有一个树莓 Pi 和一个 Adafruit TFT，你就已经成功制作了你自己版本的[【戴夫】的 PiPhone](http://www.davidhunt.ie/piphone-a-raspberry-pi-based-smartphone/) 。

这种美味的概念验证蜂窝三明治是通过在 Pi/TFT 硬件中添加一个通过 UART 通信的 [Sim900 GSM/GPRS 模块](http://wm.sim.com/producten.aspx?id=1019)来制作的，同时在中间使用一块泡沫芯板来防止短路。你不会得到免费服务或任何东西，但你可以把一张预付费 SIM 卡塞进去。他用一个[脂肪电池](http://www.adafruit.com/products/328)为它供电，并使用一个直流到 DC 转换器来设置 3.7V 到 5V。你可以做得比 158 美元的炸弹更糟糕，我们打赌你已经有一个私家侦探了。我们希望更多的手机有婴儿摇杆开关。

PiPhone 有一个小问题:它变得相当热，没有太多空间让空气流通。为了获得最佳效果，让它在精心打理的窗台上冷却，或者像[戴夫]那样在风扇附近操作。在撰写本文时，他还没有在 GitHub 上发布代码，但他将屈服于高需求。跳起来看看[Dave]的 PiPhone 之旅，看他用它打电话。

[https://www.youtube.com/embed/8eaiNsFhtI8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8eaiNsFhtI8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[感谢 Polossatik 通过 [The Inquirer](http://www.theinquirer.net/inquirer/news/2341680/linux-engineer-builds-raspberry-pi-piphone-for-usd158) 通过 [Raspberry Pi Foundation](http://www.raspberrypi.org/piphone-home-made-raspberry-pi-smartphone/) 提交此文]