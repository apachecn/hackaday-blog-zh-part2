# 用微控制器读取裸 NAND 闪存芯片

> 原文：<https://hackaday.com/2012/09/20/reading-bare-nand-flash-chips-with-a-microcontroller/>

NAND 闪存，从 USB 拇指驱动器到非常昂贵的固态硬盘驱动器，同样的存储芯片越来越常见。由于它们(部分)用作手机、Wii、路由器和几乎所有消费电子设备的存储设备，你很可能同时被几十个 NAND 芯片包围。

几年前，杰出的黑客[Sprite_tm]建立了一个版本，他能够使用 PC 并行端口读取 NAND 闪存芯片的内容。在个人电脑上找到一个并行端口变得越来越难了，所以[他更新了他的版本](http://spritesmods.com/?f=had&art=ftdinand)来从 USB 端口读取闪存芯片。

[Sprite_tm]的构建有两个主要组件。首先，为了读取闪存芯片，他需要一种方法来断开非常小的 TSOP48 封装上的引脚。[Sprite]在易贝找到了一个适合这些芯片的小巧插座，价格约为 10 欧元。

通过 USB 与闪存芯片通信有点困难。[Sprite]知道他需要 USB 2.0，但没有多少微控制器实现了这一点。幸运的是， [FTDI FT2232H](http://www.ftdichip.com/Products/ICs/FT2232H.htm) 具有 USB 2.0，以及能够直接从闪存芯片读取数据和地址引脚的非常好的功能。经过一点焊接，[Sprite_tm]留下了上面看到的设备。

[Sprite_tm]找到了[一个不错的库](http://www.intra2net.com/en/developer/libftdi/)来 bitbang FTDI 芯片上的管脚，一次从 Flash 芯片请求一页内存。这款设备像宣传的那样工作，但速度仍然有点慢，只有 250 kBps。[Sprite]认为他可以通过一次请求多个页面来提高读取闪存芯片的速度，但这仍然比旧的并行端口解决方案快几个数量级。

有一个很好的软件[Sprite]可以帮助他(可能还有其他人)通过 USB 读取裸 NAND 闪存芯片。这意味着，如果你有一个损坏的 USB 闪存驱动器或 SD 卡，它可以解除芯片的焊接，并用你自己的控制器读取它。将从闪存驱动器恢复的数据块解释为文件系统是另一回事，但这仍然是一个相当了不起的构建。