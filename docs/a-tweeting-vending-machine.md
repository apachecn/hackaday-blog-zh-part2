# 推特自动售货机

> 原文：<https://hackaday.com/2015/02/10/a-tweeting-vending-machine/>

[齐格鲁德]设法从他宿舍得到一台旧的自动售货机。唯一的问题是主板上的微控制器坏了。他和他的朋友决定他们最有可能让机器恢复正常工作，但他们也知道他们可能会对它进行一些升级。

这个系统使用两个 Arduino Pro Minis 和一个电动 Imp 来填充所有的新功能。一个 Arduino 连接到机器的原始主板。Arduino 与一些移位寄存器、继电器和电压调节器接口。只要特定的饮料不是空的，这个微控制器也会点亮机器上的按钮。它控制七段 LED 显示屏，以及读取硬币验证器。

该团队不得不对最初的[硬币验证器](http://hackaday.com/2013/08/20/hacking-coin-collection/ "Coin Accepter")进行逆向工程，以便弄清楚机器是如何检测和计数硬币的。一旦他们想出如何读取硬币的状态，他们还建立了一个定制的驱动板来驱动螺线管。

第二个 Arduino 用于使用 Mifare RC522 读卡器读取 NFC 和 RFID 卡。该系统使用自己的信用系统，因此可以向用户发放具有一定金额预付费信用的卡。一旦出售了饮料，它将适当地扣除信用。两个 Arduinos 通过串行通信。

该团队还希望这台机器能够与外界通信。在这种情况下，这意味着发送厚脸皮的推文。他们最初为此使用了一个 Raspberry Pi，但发现 SD 卡不断损坏。他们最终换了一台[电动 Imp](http://hackaday.com/2012/09/04/hands-on-with-the-electric-imp/ "Electric Imp") ，效果不错。Arduino 每分钟都会向 Imp 发送状态更新。如果状态发生变化，例如饮料被分发，那么 Imp 将发送一条 tweet 让世界知道。如果出现堵塞或某个特定的插槽变空，它还会向维护人员发送推文。

[https://www.youtube.com/embed/gayukPKz96c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gayukPKz96c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)