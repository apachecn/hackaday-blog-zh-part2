# 观看 Windows 更新:FTDI 驱动程序正在杀死假芯片

> 原文：<https://hackaday.com/2014/10/22/watch-that-windows-update-ftdi-drivers-are-killing-fake-chips/>

FTDI FT232 芯片出现在成千上万的电子产品中，从 Arduinos 到测试设备，以及许多消费电子产品。这是一个简单的芯片，将 USB 转换为串口，但非常有用，可能是地球上最克隆的硅片之一。多亏了最近的一次 Windows 更新，所有那些假的 FTDI 芯片都有被砖化的危险。这不是假的 FTDI 芯片插在运行最新 FTDI 驱动的机器上就不能工作的情况；最新的驱动程序*用砖块*伪造芯片，使它们无法与*的任何*电脑一起运行。

关于 FTDI 芯片问题的报告[于本月初浮出水面](http://forum.arduino.cc/index.php?topic=270175.0)，对这一行为的解释出现在[一个 EEVblog 论坛的帖子](http://www.eevblog.com/forum/reviews/ftdi-driver-kills-fake-ftdi-ft232/)中。来自 FTDI 的这些芯片的新驱动程序通过最近的 Windows 更新交付，将 USB PID 重新编程为 0，这是 Windows、Linux 和 OS X 不喜欢的。这使得任何操作系统都无法访问该芯片，有效地阻止了任何碰巧拥有这些假冒 FTDI 串行芯片的设备。

由于 FTDI USB 转 UART 芯片非常普遍，市场上充斥着克隆和假冒产品。通过看包装很难区分真假版本，但是看一看硅片[就会发现巨大的差异](http://hackaday.com/2014/02/19/ft232rl-real-or-fake/)。FT232 的新驱动程序利用了这些差异，对其进行了重新编程，使其无法与现有驱动程序一起工作。对于 FTDI 来说，这是一个减少硅伪造者的大胆策略。一家讲道理的 T2 公司会追查假芯片的制造商，而不是那些很可能不知道他们有假芯片的消费者。

此驱动程序更新的解决方法是从 WinXP 或 Linux 机器上的 FTDI 网站下载 FT232 config [工具，更改假芯片的 PID，并且永远不要在现代 Windows 系统上使用新驱动程序。肯定会有一个自动工具来自动修复这些芯片，但在此之前，请仔细看看 Windows Update 正在安装什么——仅凭外观很难判断您的设备是否有假的 FTDI 芯片。](http://www.ftdichip.com/Support/Utilities.htm)