# 使用 EBay 提供的 ARM + LCD 开发板进行开发

> 原文：<https://hackaday.com/2012/11/07/developing-with-ebay-sourced-arm-lcd-dev-boards/>

![](img/16fce36223f2fd701d7fba14a9be0109.png "TFT")

易贝不仅仅是假冒的名牌手袋和一盒盒全棉花糖幸运符，有时还真有一些有用的东西出售。[Matt]在托架上发现了一堆带有集成 LCD 显示器的中国制造的 ARM 开发板，但是如果没有可靠的工具链，这些开发板——尽管很酷——几乎毫无用处。谢天谢地，[他想出了如何用这些板子](http://zizzle-brewbot.blogspot.com/2012/10/stm32-lcd-touch-screen-demo.html)做些什么，并且把所有东西整齐地打包成一个 VirtualBox 映像。

这些主板通常包括一个 2.4 英寸或 3.2 英寸的触摸屏液晶显示器，一个 STM32F103 ARM Cortex-M3 CPU，一个 microSD 卡连接器，有时还有一些其他的好东西，如 16MB 的闪存和一个 RS-232 端口。一个易于使用的外形中包含了惊人的计算能力，40 美元的价格使其更加令人惊叹。

因为这些主板提供的远不止一个普通的 Arduino，所以一个合适的操作系统是合适的。[Matt]浏览了一下[freer tos](http://www.freertos.org/implementation/a00002.html)，包括了一些他的基于 Ubuntu 的 VirtualBox 映像~~的演示程序(可以在[Matt]的网站上下载，这是一个 dropbox，如果你需要一些托管，请发邮件给我们，[Matt])~~没关系，请看下面。

对这些电路板进行编程可以通过串行接口完成，但是像 [Bus Blaster](http://dangerousprototypes.com/docs/Bus_Blaster) 这样的 JTAG 程序员让事情变得非常非常简单。

休息之后你可以看看 Matt 做的一些演示。这是一个非常酷的开发，比 Raspberry Pi 或其他高功率 ARM 板更适合集成到电子项目中，我们希望在未来看到更多。

编辑:你知道托管 Linux 发行版的真正好处是什么吗？[激流。那是[Matt]的发行版，HaD 的工作人员正在播种。请播种。](https://thepiratebay.se/torrent/7803003)

[https://www.youtube.com/embed/KdvOsVIG_PQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KdvOsVIG_PQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)