# Hackaday 复古版:并行端口以太网

> 原文：<https://hackaday.com/2014/04/16/hackaday-retro-edition-parallel-port-ethernet/>

又到了对成功装载了我们复古版的[古老硬件进行综合报道的时候了。这一次是完全随机的，完全没有计划的以太网适配器并行端口综述。](http://retro.hackaday.com/)

* * *

首先是[Tom Moss] [带着他的 IBM 5150](http://hackaday.com/?p=120114&preview=true#jp-carousel-120119)——第一台“IBM 兼容”的家用电脑，i7 boxxen 的前身，当你读这篇文章的时候，它正在温暖你的脚踝。这台机器标配了一个 4.77 MHz 8088 CPU，8087 FPU，512k RAM，两个 360k 5.25”软盘驱动器，以及一些非常酷的附加功能:一个 ISA 到 CompactFlash 卡适配器，为[Tom]的机器提供 4GB 的存储空间。

[汤姆]是如何连接到互联网的？Xircom PE3-10BT 网络适配器。这个精巧的装置将任何并行端口变成了以太网。通过 Telnet 程序，[Tom]能够连接到 Unix 系统，并使用 Lynx 浏览复古网站。他还没有安装 DOS 浏览器，但是 FTP 已经可以使用了，这使得他可以直接将古老的软件下载到他巨大的 CF 卡上。

下一个不是很经典，但它确实将过时硬件的精神带到了网络上。[瓦伦丁]正在 open cores 使用一个[FleaFPGA](http://www.fleasystems.com/fleaFPGA.html)和一个[186。FPGA 板给他 VGA 输出、SD 卡、PS/2 键盘，但没有联网选项。这对[瓦伦丁]来说不成问题，因为](http://opencores.org/project,next186_soc_pc,overview)[他将一个 Xircom PE3 并行端口连接到以太网适配器](http://hackaday.com/?p=120114&preview=true#jp-carousel-120118)。是的，与上面的 5150 相同的适配器。[Valentin]说他的并行端口技术有点混乱，没有双向和专用的 IRQ 硬件支持。不过，这很管用，所以我们不能因此责怪他。

我们一直在寻找那些在旧硬件上装载了我们复古版的人。如果你有一些过时的硬件放在阁楼上，把它拿出来，装上 Hackaday Retro，然后送进去。

下面是来自[汤姆]和[瓦伦丁]的图片。

 [![FleaFPGA_Ethernet_Hack1](img/3b41307211f7b71409bf4b28a9c79676.png "FleaFPGA_Ethernet_Hack1")](https://hackaday.com/2014/04/16/hackaday-retro-edition-parallel-port-ethernet/fleafpga_ethernet_hack1/)  [![FleaFPGA_Ethernet_Hack2](img/ad7ac05fd32c2d59cc7b76446f87189a.png "FleaFPGA_Ethernet_Hack2")](https://hackaday.com/2014/04/16/hackaday-retro-edition-parallel-port-ethernet/fleafpga_ethernet_hack2/)  [![IMG_4321](img/5d5a647c54e3bedb57f85b66770eaad3.png "IMG_4321")](https://hackaday.com/2014/04/16/hackaday-retro-edition-parallel-port-ethernet/img_4321/)  [![IMG_4322](img/d5a5a78f602ad567d0fff71edf0b5ad3.png "IMG_4322")](https://hackaday.com/2014/04/16/hackaday-retro-edition-parallel-port-ethernet/img_4322/)  [![IMG_4320](img/479ad098f4482fb82cf527a96062cc1e.png "IMG_4320")](https://hackaday.com/2014/04/16/hackaday-retro-edition-parallel-port-ethernet/img_4320/)