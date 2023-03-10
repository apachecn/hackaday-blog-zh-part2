# ContactKey:一个便携式电池供电的电话簿

> 原文：<https://hackaday.com/2013/09/22/contactkey-a-portable-battery-powered-phonebook/>

![contactKey](img/9355cb691a60a55be646f080f8e3db11.png)

虽然它还是一个原型，[Russell]向我们透露了他的电池供电的[设备，用于存储你的联系人列表:ContactKey](http://www.youtube.com/watch?v=HZ1KTiWjuhQ) 。(警告:声音大@开头)。当然，纸张可以备份你的联系信息，但纸张远没有炫耀的那么酷，也不能直接从你的 Android 接收更新。ContactKey 在有机发光二极管屏幕上显示一个联系人的信息，你可以通过按几个按钮来选择:向上、向下或重置。虽然向上/向下按钮可以一次前进一个联系人，但按住一个按钮会以闪电般的速度在列表中穿梭。几秒钟的不活动会导致超时，并使 ContactKey 进入睡眠状态以节省电池寿命。

该构建使用 ATMega328 微控制器和外部 EEPROM 来存储实际列表。[Russell]编写了一个 Android 应用程序，它可以通过 FTDI 芯片将您的联系人列表同步到 USB 上的 ContactKey。微控制器使用 I2C 与 EEPROM 通信，而有机发光二极管显示器通过 SPI 与 ATMega 接口。我们期待着看到[Russell]一旦脱离试验板，ContactKey 会有多紧凑；大多数智能手机的电池寿命并不是特别出色。未来的手机最终会更长寿，但我们打赌不会是这一款。

[https://www.youtube.com/embed/HZ1KTiWjuhQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HZ1KTiWjuhQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)