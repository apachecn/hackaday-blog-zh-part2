# 树莓派和 Windows 10 物联网核心:一个巨大的失望

> 原文：<https://hackaday.com/2015/08/13/raspberry-pi-and-windows-10-iot-core-a-huge-letdown/>

去年春天，微软公布了他们的 Windows 和物联网计划。它始于 Raspberry Pi 和 Windows 10 物联网核心——一个在 ARM 架构上运行的 Windows API 调用的精简系统。是的，微软终于在远离桌面，为十亿个物联网事物建立一个平台，或者填补数万个运行 XP 的 POS 终端和 ATM 被离线留下的空白。哪一个都是准确的。

本周早些时候，微软[宣布首次公开发布 Windows 10 物联网核心](https://blogs.windows.com/buildingapps/2015/08/10/hello-windows-10-iot-core/)。这是评论，但这里的外卖:运行。尽可能快地逃离 Windows IoT。除非你有为 Windows 编写应用程序的强烈愿望，否则这不值得你浪费时间，即使这样，你也可以用任何 Linux 发行版不费吹灰之力做得更好。

当 Windows 10 IoT 首次公布时，人们对类似 Windows RT 的体验寄予厚望。能够在 Raspberry Pi 上运行真正的 Windows 应用程序将是一个杀手锏，在 Pi 上安装 Skype 将意味着真正的 *Jetsons* 风格的视频电话将很快出现。

Windows 10 物联网核心与其说是一个操作系统，不如说是一个将运行用 Windows APIs 编写的应用程序的设备:没有外壳。如果您想控制几十或几百台设备，每台设备都运行一个用 Visual Basic、JavaScript、C#或 Python 编写的程序，这正是您所需要的。

[![devicemanager](img/32088417bf3f91c761bb74fe97777cba.png)](https://hackaday.com/wp-content/uploads/2015/08/devicemanager.png) 与 Windows 10 物联网核心的大部分交互都是通过网络进行的。在启动并将浏览器指向 Pi 之后，您会看到一个相当完整的基于 web 的界面。在这里，您可以检查哪些设备连接到 Pi，查看正在运行的进程，以及运行新的应用程序。可以把这个功能想象成一个基于网络的 Windows 控制面板。

虽然 Windows 10 IoT 在 Pi 上使用 HDMI 输出，但这仅仅是信息性的，Pi 的视频输出功能是为特定应用显示器保留的，数字标牌、POS 终端和 ATM 是 Windows 10 IoT Core 擅长的领域。对于通用计算，你最好去别处看看。

### 安装

官方表示，安装 Windows 10 物联网核心的唯一方法是使用运行 Windows 10 的计算机。GitHub 上的 ffu2img 项目有几种解决方法。这个 Python 脚本采用了特殊的 Microsoft。FFU 图像文件格式，并把它变成一个。IMG 文件，可以在*nix 下与 dd 一起使用，在 Windows 上与 Win32DiskImager 一起使用。

是的，Windows 10 对每个拥有相对现代的 Windows box 的人来说都是免费的，但由于运行 Windows 10 物联网核心的唯一要求是在 SD 卡上放置一个映像并监控一群物联网核心设备，因此没有理由为什么这个操作系统不能以一种方式提供。IMG 档案。

将映像放在 SD 卡上后，安装 Windows 10 物联网核心就像任何其他 Raspi 发行版一样简单:将卡插入 pi，连接以太网电缆，并给它一些电源。不，你不需要键盘或鼠标；你实际上对 Pi 能做的事情很少。事实上，通过 Pi 的 HDMI 端口显示的唯一内容是一个屏幕，显示 IP 地址和连接的 USB 设备。

[![PiWin](img/7951374f4d8607aea52605394c238bce.png)](https://hackaday.com/wp-content/uploads/2015/08/piwin.png)

The totality of the Windows 10 IoT Core experience

您确实有一些语言和网络设置选项，也有一些教程和示例——连接到 Visual Studio 和闪烁 LED——但仅此而已。Windows 10 物联网核心的基础用户体验只是网络信息、设备名称和一张树莓派的图片。

树莓派的 Windows 10 物联网核心有几个缺点。官方上，[唯一支持的 WiFi 模块](http://ms-iot.github.io/content/en-US/win10/SetupWiFi.htm#WiFi_Devices)是[官方的 Raspberry Pi WiFi 模块](http://swag.raspberrypi.org/collections/frontpage/products/official-raspberry-pi-Wifi-dongle)，采用 BCM43143 芯片组。到目前为止，最受欢迎的用于 Raspberry Pi 的 WiFi 模块(也是你应该一直放在包里的东西)是 Edimax EW-7811Un，这是一个使用 Realtek 芯片组的微型 WiFi 模块[。很有可能，如果你有一个树莓 Pi 2，你拿起的那个 WiFi 模块就不能用了。常识告诉我们可以为 Realtek 芯片组安装 Windows 驱动程序，但事实并非如此；没有任何 Windows 驱动程序可以与 Windows 10 物联网核心兼容。甚至来自 Raspberry Pi 基金会的设备，如 Raspberry Pi 摄像头，也不被物联网核心支持](https://wikidevi.com/wiki/Edimax_EW-7811Un)

如果你曾经想要更清楚的证据，证明 Windows 10 物联网核心并不意味着像其他基于 Linux 的单板计算机一样是一个可扩展的系统，你只需要稍微深入一点。数字音频完全被忽略，引脚 8 和 10(通常为每隔一个 Raspberry Pi 分配的 3.3V UART 保留)是保留引脚。微软设法制造了一台没有硬件 UART 的单板计算机。

幸运的是，其中一些问题是暂时的。Windows On Devices 团队的一名代表告诉我们，未来将支持更多的 WiFi 加密狗；他们唯一能及时找到的驱动程序是 Raspberry Pi 基金会的官方加密狗。工程权衡的类似情况是缺乏 UART 支持的原因。

### 这到底是给谁的？

微软将推出一个不支持事实上的标准 WiFi 适配器、硬件 UART 或大多数外围设备驱动程序的非操作系统是一回事。把这个卖给“创客运动”会让人难以置信。还有一种解释。

[![Corewatcher](img/6f26e721502a504c2341c5bfc9597eab.png)](https://hackaday.com/wp-content/uploads/2015/08/corewatcher.png)

The Windows 10 IoT Core Watcher, the remote admin app for multitudes of Pis.

让我们再次回顾一下 Windows 10 物联网核心到底是什么。通过设计，你可以在 Visual Studio 中编写程序，并将其上传到一个或多个运行物联网核心的设备上。这些程序可以有一个看起来熟悉的 GUI，并且实际上非常容易构建，因为 Windows 框架开发已经有 20 多年的历史了。这不是为制造商设计的设备，这是为销售终端和自动取款机设计的设备。windows XP——仍在数量惊人的自动取款机上使用的操作系统——即将消失，这是微软试图挽救他们在该市场的份额。物联网核心不适合你，也不适合我，更不适合想眨一下 LED 灯的 9 岁小孩。这是一个为那些需要替换成千上万仍然运行 XP Embedded 的系统，并且需要在信息亭和终端中使用 Windows APIs 的公司设计的操作系统。

### 保存您的 SD 卡

对于任何一个拥有 Raspberry Pi 2 和 SD 卡的人来说，你在试用 Windows 10 物联网核心时唯一的投资就是你的时间。不值得。

虽然 Windows 10 物联网核心对任何有大量 Visual Basic 和其他工程债务的公司来说都很棒，但它不适合黑客、制造商或任何开发新事物的人。为此，如果你想要一个可以远程编程和更新的联网盒子，有几十种选择。用于 Pi 和 BeagleBone 的 [Cloud9 IDE](https://c9.io/) 允许你在单板计算机上编写代码，而不必强迫你安装 Visual Studio，Linux 是管理互联网上几十或几百个机器的王者。

这不是一个可以取代一切的操作系统。Linux 系统几乎总是有更好的硬件支持，在嵌入式设备上尤其如此。Windows 10 物联网核心是一个开始，应该如此看待。它是为那些想要它的人准备的，但对其他人来说，十几个 Linux 发行版中的任何一个都会更好。