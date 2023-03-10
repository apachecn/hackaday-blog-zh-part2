# 比格波恩绿色实践:更低的价格，相同的马力

> 原文：<https://hackaday.com/2015/08/05/beaglebone-green-hands-on-lower-price-same-horsepower/>

虽然 BeagleBone Green 在去年 5 月的湾区创客大会上宣布，但在通常的论坛和 IRC 频道上并没有太多关于它的谈论。现在，它终于出来了，我得到了其中的一个。通过 BeagleBoard 基金会和 Seeed 工作室之间的合作，用小型 Linux 板做*实际工作*的最好的小型 Linux 板现在更便宜，更现代，也更绿色。

BeagleBone Green 是基于 TI ARM Cortex-A8 的开发板 BeagleBone Black 的升级版。这是一台非常强大的机器，具有一些有趣的功能，使其成为嵌入式应用的完美设备。随着 BeagleBone 绿色，BB 黑色得到了一个小的硬件更新和价格大幅下降。如果你想在 Linux 板上做真正的工作，这是一个很好的选择。查看下面的评论，了解所有更新的内容，所有不变的内容，以及为什么这是近年来小型 Linux 主板最有趣的发展之一。

### 与比格犬骨黑色的区别

[![BlackVGreen](img/cc8cb9ba7c411d84e02aa2d39a153e70.png)](https://hackaday.com/wp-content/uploads/2015/08/blackvgreen.jpg)

The BeagleBone Black and BeagleBone Green back to back

BeagleBone Black 已经存在两年多了，但它仍然是一台非常强大的机器。BeagleBone Green 大量借鉴了黑色，做了一些改动以满足降低成本的目标，并使 BB Green 更容易使用。

到目前为止，最大的变化是取消了 microHDMI 连接器。与此同时，电路板上出现了一大片空白区域，而恩智浦 HDMI 成帧器芯片曾经位于 BB Black 上。当我与[Jason Kridner]交谈时，他对取消 Green 的 HDMI 功能的解释是“没有人使用它。”这是公平和真实的；如果你想要一个媒体服务器，你可以得到一个树莓派，如果你想要一个小巧的 Linux 盒子来快速切换引脚，你可以得到一个 BeagleBone。HDMI 的取消发挥了 BeagleBone 的优势，使它成为一个更便宜的主板。你不能否认这一点。

变化列表中还增加了两个 Grove 连接器。这些连接器是模块化电子系统的一部分，将 UART 或 I2C 总线放在一个连接器上。有了这些连接器和 Grove 系统的一些模块，构建简单的项目变得轻而易举。增加两个 Grove 连接器——一个 UART，一个 I2C——是 Seeed 对 BeagleBone Green 的最大贡献，并且有一个从简单的逻辑门到有机发光二极管显示器和 GPS 模块的大型零件目录，它非常方便。

[![oled](img/3f7c75cc19e4d1f389b8fa026a5a777e.png)](https://hackaday.com/wp-content/uploads/2015/08/oled.png)

Grove modules, like this OLED display, are plug and play with the BeagleBone Green

除了这些变化，绿色的比格骨和黑色的比格骨几乎完全一样。它拥有与 BB Black 相同的内存容量、相同的处理器、相同的 eMMC 闪存容量和相同的引脚排列。绿色移动到 USB 微型连接器，用于电源和串行连接。这是黑色猎兔犬上的 USB 迷你。这是一个期待已久的可喜变化。电源的桶形插孔已经从 BeagleBone Green 上移除，更大的 USB 端口已经移到以太网插座旁边。

就像 BeagleBone 的黑色一样，绿色来自已经安装在 eMMC 的 Linux 映像上的 [Cloud 9 IDE](https://c9.io/) 。这是一个基于云的 IDE，但是托管在 BeagleBone 上。对于一个不是台式电脑的设备来说，这是在一个小小的 Linux 机器上运行代码的最简单的方法。将它与串行终端结合起来，这就是您所需要的一切。

### 为什么它很棒

虽然 BeagleBone Black 已经存在了一段时间，BeagleBoard 甚至更长，但 Beagles 一直是树莓 Pi 的副手。这是一种耻辱。如果你想实时控制很多管脚，Raspberry Pi 并不是理想的工具，Pi 上的 GPIO 扩展更像是一个杂牌，而不是它的设计目标。

相比之下，beagle bone——带有花哨的 PRUs——是为在 Linux 下运行 GPIOs 而设计的，速度非常快。它已经被[用作一台旧 Mac 电脑](http://hackaday.com/2014/02/05/the-30th-anniversary-macintosh/)的显卡，并驱动[数量惊人、令人眼花缭乱的 RGB led](https://hackaday.io/project/3-fled)，以及数以千计其他有趣和核心的项目。

在 BeagleBone Green 中移除 HDMI 端口不会降低该板的功能。就像我上面说的，反正没人用。此外，你可以为 BBG 买一个 LCD 斗篷，并让它与 3D 加速器一起工作，你真的不会失去任何功能，只是价格降低了 16 美元。BBG 将以 39 美元的价格上市，大约相当于树莓派的价格。虽然它不会给许多想要一个廉价的 Linux 盒子来进行复古视频游戏仿真的人留下深刻印象，但对于任何想要完成真正工作的人来说，它都是一个很好的主板。