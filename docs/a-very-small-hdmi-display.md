# 非常小的 HDMI 显示屏

> 原文：<https://hackaday.com/2013/07/08/a-very-small-hdmi-display/>

随着几十个带 HDMI 的口袋大小的 ARM 板的出现，我们很惊讶我们以前没有见过这种情况。[Elias] [制作了一个定制的驱动板](http://hipstercircuits.com/finally-a-working-4-3-hdmi-compatible-lcd/)，它可以从手机上接收 HDMI 输入，并将其显示在一个非常小的高分辨率显示器上。

所使用的显示器与 HTC desire HD 的库存相同。分辨率为 800×480，对于基本的台式机来说绰绰有余，尽管它不是少数旗舰手机的 1080p 怪物，但对于大多数用途来说也绰绰有余。

[Elias]板由一个 Himax 显示驱动器和一个 TI DVI 接收器组成。板上包括一个 MSP430 微控制器，用于初始化驱动器和显示器。这个版本最初是为 [Replicape](http://replicape.com/) 设计的，这是一个用于 Beaglebone 的 3D 打印机驱动板，但因为到这个板的唯一连接是 HDMI 和一个到‘430 的 SPI，所以它也适用于 Raspberry Pi。