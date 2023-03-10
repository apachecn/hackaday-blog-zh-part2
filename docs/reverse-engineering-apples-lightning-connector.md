# 逆向工程苹果的 Lightning 连接器

> 原文：<https://hackaday.com/2015/02/14/reverse-engineering-apples-lightning-connector/>

近两年半前随着 iPhone 5 推出的苹果 Lightning 连接器阻碍了令人难以置信的自制电子产品场景，此前人们习惯于更大、更旧、更好记录和更开放的 30 针连接器。现在，终于，[苹果 Lightning 连接器内部的协议被破解了](http://ramtin-amin.fr/#tristar)。我们离 Lightning 分线板还有一段距离，但这是第一次证明串行控制台可以通过 Lightning 连接器获得。这是完全拥有一个设备的第一步，这就是所有这些利用将如何开始。

[Ramtin Amin]像大多数逆向工程任务一样，开始拆卸 Lightning 连接器，查看专利，寻找连接器的来源，以及使用类似硬件的任何其他产品。[Ramtin]发现了一个由 STM32 微控制器供电的闪电串行转换器。拆卸固件并查看逻辑分析仪上的输出，[Ramtin]找出了协议的一部分，大部分布线，并在一些研究后，找到了 Lightning-enabled iProducts 中一个迄今尚未确定的芯片是如何布线的示意图。

这款芯片俗称 Tristar，更准确地说是 CBTL1608A1。在 iPhone 5 发布会的拆机热潮中，这种芯片经常被认为是显示端口多路复用器。它是一个 mux，但不是用于 display port——它仅用于连接附件(Lightning) UART、调试 UART、基带、SoC 和 JTAG。这是城堡的钥匙，能够通过这个芯片意味着我们现在可以拥有自己的设备。

该芯片是一个小得令人难以置信的 BGA 事件，它[Ramtin]脱焊，回流到分线板上，并连接到 STM32 发现板。利用他在其他支持闪电的硬件上使用的技术，[拉姆丁]能够连接他的 iPhone，并稍微窥视他的设备的内部工作。

它还不能完全控制一个设备，但这将是所有未来开发的开始。[Ramtin]上传了一个短视频作为概念验证，您可以在下面查看。

[https://www.youtube.com/embed/hHdDslVI7O0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hHdDslVI7O0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)