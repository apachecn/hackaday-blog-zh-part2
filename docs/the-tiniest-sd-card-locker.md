# 最小的 SD 卡柜

> 原文：<https://hackaday.com/2014/01/18/the-tiniest-sd-card-locker/>

![sdlocker-tiny](img/88cf308fadc963492dbcc7f68a2c4203.png)

如果你没有意识到，你的 SD 卡上的写保护开关可能不会做任何事情。它只是一个开关，真的，如果一个 SD 卡读卡器懒得把那个信号发送到你的电脑，那它就完全无效。接下来的问题是，你的操作系统实际上对写保护信号做了什么。

对 SD 卡进行写保护的更好方法是使用 SD 卡控制器上的 TMP_WRITE_PROTECT 位。[Nephiel] [想出了一个令人惊讶的小装置来设置位](https://github.com/Nephiel/sdlocker-tiny)，整个电路安装在一个旧的 Playstation 存储卡内。

[Nephiel]基于我们去年年底看到的[Karl Lunt]的[sd 卡柜](http://hackaday.com/2013/11/12/keep-your-sd-cards-data-safe-with-the-sd-locker/)进行他的项目。[Karl]的 SD Locker 使用 ATMega328 微控制器、一对 AA 电池和一个 SD 卡插座来执行位切换。这仍然是一个非常小的装置，可以放在一个 Altoids 罐里，但是[Nephiel]认为他可以把它做得更小。

新的改进版本使用 ATTiny85 对 SD 卡进行 SPI 访问。一个按钮和 LED 作为用户界面:LED 关闭时，SD 卡是可写的。按下按钮，卡被锁定，LED 灯亮。