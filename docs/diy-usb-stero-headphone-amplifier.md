# DIY USB 立体声耳机放大器

> 原文：<https://hackaday.com/2015/01/22/diy-usb-stero-headphone-amplifier/>

最大和最好的音响发烧友项目通常是巨大的电子管放大器，巨大的扬声器驾驶室，或其他同样令人印象深刻的东西。然而，事情并不总是这样，正如[lowderd]用[演示的那样，一个小小的 DIY USB DAC](http://imgur.com/a/jNh1E) 可以将 USB 端口变成耳机输出。

在过去，将 DAC 放在 USB 总线上需要一些相当昂贵的硬件和大量的技能。如今，你只需[买一个单芯片 USB 立体声 DAC](http://www.ti.com/product/pcm2707) 就可以了，它仍然具有非常好的规格。[lowderd]使用 TI PCM2707 USB DAC，这是一种识别为 USB 音频 1.0 类设备的芯片，因此它在 Windows 或 OS X 中工作都不需要驱动程序。

该电路安装在一个微小的 PCB 上，一侧有一个 USB 端口，另一侧有一个耳机插孔，芯片和所有相关元件位于两者之间。芯片上有一些引脚可以调节音量、播放/暂停。和 skip，但为了简单起见，这些引脚没有连接。

板子是在奥什公园制作的，第二次修改是由波诺科用竹子和丙烯酸激光切割出来的。这是一个看起来很棒的小盒子，正好可以放在[罗德]的耳机盒里。