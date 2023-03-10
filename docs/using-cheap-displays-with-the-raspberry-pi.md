# 在树莓派上使用廉价的显示器

> 原文：<https://hackaday.com/2015/03/05/using-cheap-displays-with-the-raspberry-pi/>

Raspberry Pi B+有一个原生 VGA 连接。当然，它隐藏在二进制 blobs 和设备树中，你需要正确连接 GPIO 引脚*和*,但是可以将 VGA 监视器连接到 Raspi B+。对于勇敢、聪明或愚蠢的人来说，这意味着你也可以驱动原始的 DPI 显示器。[Robert]有一些这种非常便宜的显示器放在[周围，并决定尝试一下整个事情](http://blog.reasonablycorrect.com/raw-dpi-raspberry-pi/)。这很有效，他已经写下了怎么做。

Raspberry Pi 的芯片架构师之一 Gert van Loo 在设计 Pi 时非常聪明。芯片中有一个并行接口，当与几十个电阻结合时，[可以驱动 VGA 显示器*以及 HDMI 显示器*](http://hackaday.com/2014/09/10/raspberry-pi-gets-vga-dual-screen-support/)的。具有显示并行接口的屏幕实际上非常类似于 VGA 规范所要求的。问题是，几乎没有任何关于树莓派的记录，找到它意味着在论坛中搜索。

[Robert]的示例电路使用了来自 Adafruit 的一个 5 英寸显示器，[一个 40 针分线点](https://www.adafruit.com/products/1932)和一束原型导线。设置需要[抓取用于 Raspi VGA 分线板的设备树的精简版本](https://github.com/robertely/dpi666/blob/master/setup/dt-blob-dpi.dts)，设置输出格式、rgb 顺序和显示器的纵横比，并连接所有设备。

有趣的是[Robert]从头开始复制了这个项目，并发现任何带有 40 针 DPI 连接器的显示器都可以与 Raspi 一起工作，前提是您有数据表。这很酷。这些显示器可能很便宜，因为我们还没有一个合适的 Pi 显示器，所以现在只能这样了。

下面的视频是[罗伯特]对这个建筑的灵感。

[https://www.youtube.com/embed/DTuvzxkVaKs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DTuvzxkVaKs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)