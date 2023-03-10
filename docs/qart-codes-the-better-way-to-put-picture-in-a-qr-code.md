# QArt 码，将图片放入 QR 码的更好方法

> 原文：<https://hackaday.com/2012/04/13/qart-codes-the-better-way-to-put-picture-in-a-qr-code/>

[![](img/286b2875c6649ddc4f51bf1a67172afe.png "QR2")](http://hackaday.com/wp-content/uploads/2012/04/qr2.png)

现任谷歌员工、前贝尔实验室员工罗斯·考克斯(Russ Cox)发布了一个很棒的指南，教你如何将图片放入二维码。与我去年 8 月写的这个[可怕的尝试](http://hackaday.com/2011/08/11/how-to-put-your-logo-in-a-qr-code/)不同，【罗斯】的方法不仅仅是简单地将一张图像粘贴到二维码上，然后希望错误修正通过。这种新方法为每个 QR 码生成一个唯一的编码 URL。换句话说，嵌入的图像实际上是 QR 码的一部分，而不仅仅是复制和粘贴的尝试。

[Russ]hack 的基础是能够将 QR 码中包含的信息转换为 ASCII/UTF-8 或二进制编码的十进制数字。通过在将要编码的 URL 上附加一个锚标签(即`[http://swtch.com/pjw/#123456789](http://swtch.com/pjw/#123456789)...`),【Russ】可以改变 QR 码中的一整串像素，从而制作出几乎任何图像。

通过一些技巧，如构建新的里德-所罗门编码块，[Russ]可以改变 QR 码所需的像素位置。这使得 [PJW 的二进制肖像](http://spinroot.com/pico/pjw.html#123456789)的全幅图像可以显示在二维码中。

[Russ]安装了一个 [QArt 编码器](http://research.swtch.com/qr/draw)，允许任何人在任何 QR 码中放置像素化图像。[卢克·舒梅克](感谢你发来这个，[卢克])拿起这个工具，把“ol skull”n 扳手[放进一个指向 hackaday.com 的二维码](http://research.swtch.com/qr/show/4a7dfbf91f347da2)里。[Russ]做得非常好，让我的工作相形见绌。我要去角落里哭了。