# 使用 Arduino 和未更改的 CueCat 读取条形码

> 原文：<https://hackaday.com/2012/07/12/reading-bar-codes-with-arduino-and-unaltered-cuecat/>

![](img/cb60a45e092868a9fa050d9eefd7debf.png "arduino-cuecat")

[Damcave]决定尝试一些条形码阅读器项目。几年前他得到了一张支票。问题是它输出的是加密的字符集，而不是明文字符串。为了绕过这个[，他使用他的 Arduino 解密 CueCat 的数据输出](http://www.instructables.com/id/Arduino-and-CueCat-barcode-scanner)。

最初，你可以免费得到一个 CueCat。它的作用就像现在的二维码一样——你看到一个条形码，你扫描它就能找到一个网址。它从未真正流行过，但你仍然可以花大约 12 英镑买到一台。我们已经看到[项目在处理器](http://hackaday.com/2010/02/10/cuecat-meet-arduino/)上剪下一个引脚来禁用加密。但是[Damcave]不想搞乱硬件。相反，他通过 PS/2 连接器连接 Arduino，并使用软件来翻译数据。加密格式早已为人所知，因此只需将这些步骤转换成 Arduino 函数即可。