# I2C 可编程 NFC 标签

> 原文：<https://hackaday.com/2014/05/30/the-i2c-programmable-nfc-tag/>

NFC 标签很酷，但对它们进行编程以满足您的需求——无论是解锁您的电脑、制作 Arduino 自动售货机还是智能家居应用——都需要使用 NFC 设备对标签进行无线编程。一个可以用任何微控制器编程的 NFC 标签肯定会有一些有趣的应用，而[elec breaks 的 DNFC](http://www.elecfreaks.com/6730.html) 标签正好可以测试这些想法。

虽然 NFC 标签可以重新编程，但重新编程需要 NFC 控制器，无论是通过专用硬件、电话还是 Arduino 屏蔽。得益于 TI 的 RF430CL330H 动态 NFC 应答器 ic，DNFC 标签可通过带有 I2C 接口的微控制器重新编程。它仍然能做你对 NFC 标签所期望的一切——兼容 MIFARE。NDEF 读写，以及其他一切——但你可以通过 Arduino、Pi 或任何其他具有 I2C 接口的板对其进行编程。

TI 有一个关于使用 DNFC 内部芯片进行自动蓝牙配对的应用说明，Elecfreaks 自己也有一些用例，包括将 WiFi 凭据放在 Arduino 板上，而不将 SSID 放在代码和其他物联网应用中。我们认为这是一种非常有用的设备，但是对于一些我们想不出来的东西。如果你有如何使用 I2C 可编程 NFC 标签的想法，请在评论中留言。

Elecfreaks 正在为 DNFC 做一个 Indiegogo 广告，一个 13 美元。我捡了一个，不过是弹性资金，买还是不买。我不在乎。