# USB 2 串行适配器作为 I/O 设备

> 原文：<https://hackaday.com/2015/06/21/usb2serial-adapter-as-an-io-device/>

曾经有一段时间，计算机有并行端口。对于黑客类型，这意味着一个 8 位数据端口和 9 个额外的引脚，可以通过 25 引脚连接器与现实世界连接。虽然 USB 确实有助于合适的硬件，但现在情况已经不同了。[贾比]正在做一个项目，需要控制一个继电器来开关一串发光二极管。他的解决方案是使用一个 [USB 转串行适配器作为 I/O 设备](https://github.com/jabiinfante/siofus)(西班牙语，[这里翻译为](http://translate.google.com/translate?sl=auto&tl=en&u=http://blog.irontec.com/digital-io-por-las-malas-siofus/&sandbox=0&usg=ALkJrhhcR4jiCIUEzU29DgWYT2teEiGD-Q))。

他写了一个很短的 C 程序，SioFus(USB 2 Serial 的简单输入输出)，把一个简单的 USB 转串口适配器转换成一个 4 输入 2 输出的 I/O 设备。这很简单，而且能完成任务。代码使用 ioctl 并允许 DCD、DSR、CTS 和 RI 作为输入，而 DTR 和 RTS 作为输出。然后，这些引脚可能控制开关继电器的晶体管。github 上有 [SioFus 代码](https://github.com/jabiinfante/siofus)，如果你想加入的话，在【贾比】的列表上有几个待办事项。

休息后的视频应该显示了黑客的行动。看起来像某种照片亭，然后吐出一个二维码，可能是图片的 URL(如果你知道它是做什么的，请在评论中发布)。

如果你正在寻找一个更专用的硬件，看看[微型丁格斯](http://hackaday.com/2015/06/09/hackaday-prize-entry-a-bit-dingus/)——一个插入 USB 插头的微控制器，带有几个可控引脚。

[https://www.youtube.com/embed/qhWl5pRkbjI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qhWl5pRkbjI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)