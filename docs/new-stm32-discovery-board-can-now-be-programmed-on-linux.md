# 新的 STM32 发现板现在可以在 Linux 上编程

> 原文：<https://hackaday.com/2012/06/04/new-stm32-discovery-board-can-now-be-programmed-on-linux/>

![](img/8e9ba03ff93efa2a5a83fbdc025361b5.png "stm32f0-discover-linux-support")

上周三，我发布了新的 STM32F0-Discovery board 的视频评测，它是围绕 ARM Cortex-M0 芯片构建的。我推测它应该与旨在对这些发现板进行编程的开源项目一起工作。我对它进行了测试，可以建立连接，但没有代码可以刷新。所以我周末花了几个小时，加了支持。

我的更新已经在 stlink 库中[。克隆代码后，您可以使用三个命令来编译软件。/autogen.sh，。/configure，make)。这是假设您拥有所有必需的依赖项(我必须安装 libusb-1.0-0-dev)，并且您添加了文档中建议的 udev 规则(也可以在资源库中找到)。st-util 程序连接到电路板，并为 ARM 调试器提供一个监听端口(我使用的是 CodeSourcery G++ Lite 的 arm-none-eabi-gdb)。](https://github.com/texane/stlink)

当我第一次开始测试时，芯片 id 报告为 0。事实证明，针对该信息轮询的寄存器地址是错误的。在将近 900 页的参考手册中，我找到了正确存储映射器件所需的十六进制值。在那里，我还更新了 blink 示例，以生成与 Cortex-M0 芯片兼容的 ELF 文件。因此，一开始，您应该能够使用 ARM 交叉编译工具链来编译该示例，使用该实用程序连接到电路板，然后使用工具链中的调试器来连接该示例并将其闪存到 RAM。

还有很多事情要做。为了充分利用芯片，有必要在编译时使用启动文件和链接器脚本。我在这方面没有做过什么，但是我希望随着我的深入，可以做一些教程。当然，如果你自己成功地使用 Linux 机器开发了这款主板[，我们希望听到它的消息](http://hackaday.com/contact-hack-a-day/)！