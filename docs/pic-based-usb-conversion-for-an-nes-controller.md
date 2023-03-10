# 基于 PIC 的 NES 控制器 USB 转换

> 原文：<https://hackaday.com/2012/09/03/pic-based-usb-conversion-for-an-nes-controller/>

![](img/430534a5a45ad4e88f723e8e846856a8.png "pic-based-nes-usb-controller")

[Andres]来信分享了他的 USB NES 控制器项目([翻译为](http://translate.google.com/translate?hl=en&sl=auto&tl=en&u=http%3A%2F%2Ftecnologicobj12.blogspot.mx%2F2012%2F07%2Fcontrol-nes-usb-pic18f2455255044554550.html))。它枚举为一个 USB 键盘，很容易在大多数模拟器上映射。周末，我们拜访了[一个为此目的而使用的 AVR 程序员](http://hackaday.com/2012/08/31/hackaday-links-august-31-2012/)。[Andres]走了一个不同的方向，使用 PIC 微控制器，并最终将他的电路集成到控制器的主体中。

上面可以看到原型电路。[Andres]使用 PIC 18F4550 的分线板来测试电路。该芯片具有原生 USB 支持，从控制器的移位寄存器中读取按钮状态轻而易举。你可以在休息后的视频中看到他使用这个测试平台在模拟器上玩超级马里奥兄弟。

项目的第二次迭代从试验板转移到焊接电路。使用 18F2550 是因为它采用相当小的 DIP 封装。如果腿是平的，控制器外壳内就有空间放它，还有几个电容器和一个晶体。原来的控制器线被移除，以便为 USB 电缆让路。

[https://www.youtube.com/embed/f8DjpXZ5kCY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/f8DjpXZ5kCY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)