# 带 HDMI 输入的 Raspi 流光溢彩灯

> 原文：<https://hackaday.com/2014/05/18/a-raspi-ambilight-with-hdmi-input/>

随着树莓 Pi 现在以 30 美元的媒体 PC 而闻名，Pi 上 GPIO 引脚的最佳用途只能用于流光溢彩。[Great Scott Labs] [发布了一个很棒的视频](https://www.youtube.com/watch?v=tRDAzJrfZiM)关于使用 Pi 作为 Hyperion 的独特可配置流光溢彩和几乎任何可以想象的视频输入。

这不是[Great Scott]组装的第一个流光溢彩克隆，但对于第一个版本来说，流光溢彩只在 Raspbian 下工作，而不是任何随机的 HDMI 输入。新版本通过使用 HDMI 分路器盒来解决这一问题，馈入 HDMI 到复合转换器，最后馈入连接到 Raspi 的 USB 复合捕捉加密狗。

使用说明中的软件，Raspi 可以有效地镜像来自视频捕获加密狗的视频。Pi 正在运行 [Hyperion](https://github.com/tvdzwan/hyperion/wiki) 来控制一条 WS2801 RGB LEDs，使任何电视的背面闪闪发光。

由于[Great Scott]使用分量视频信号作为输入，任何设备使用这种流光溢彩所需的适配器都很容易获得。我们真诚地希望看到这个版本在旧的 Commodore 磁盘访问屏幕边框变得疯狂的情况下工作，所以如果你能工作的话，请务必[在](http://hackaday.com/contact-hack-a-day/)中发送它。

[https://www.youtube.com/embed/tRDAzJrfZiM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tRDAzJrfZiM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)