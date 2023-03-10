# 破解 IClass RFID 阅读器的更好方法

> 原文：<https://hackaday.com/2012/11/20/a-better-way-to-hack-iclass-rfid-readers/>

![](img/f014317f948e4fab5e846b208d047661.png "new-iclass-eeprom-dumper")

iClass 是一种 RFID 标准，旨在通过加密和身份验证来提高安全性。虽然它比其他 RFID 实现更安全，但仍有可能侵入系统。但是最初的 iClass 攻击是相当具有侵略性的。[Brad antonewicz]发表了一篇关于系统早期攻击的帖子，然后[展示了利用 iClass 阅读器的更好方法](http://blog.opensecurityresearch.com/2012/11/dumping-iclass-keys.html)。

我们记得大约一年半前在 27C3 的 iClass 上看过[的演讲。虽然这项技术很有趣，但它的侵入性令人难以置信。攻击者需要多个 iClass 阅读器供他使用，因为这种方法涉及重写部分固件以获得部分转储，然后将这些映像片段修补在一起。[Brad]指出，这对于现成的系统来说没问题，但高安全性安装将使用自定义映像。这意味着你需要让多个阅读器离开你试图潜入的建筑物的墙壁。](http://hackaday.com/2011/02/23/breaking-the-iclass-security/)

但他的方法不同。他设法使用 FTDI 电缆和外部电源从读取器中获取了 EEPROM 的转储。如果你想知道他是如何绕过 PIC 读取保护的，你必须深入研究他的文章中链接的源代码。