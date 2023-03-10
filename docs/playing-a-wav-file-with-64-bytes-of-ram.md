# 播放 64 字节内存的 WAV 文件

> 原文：<https://hackaday.com/2013/01/06/playing-a-wav-file-with-64-bytes-of-ram/>

![montage-final](img/9e5bd8453efca78b825b1f406a74959e.png)

[Jacques]认为他的门铃太吵了，所以第一个想到的当然是更换电子设备并在每次有人敲门时播放他选择的 WAV 文件。他最终得到的是[一个非常简洁的电路](http://picatout-jd.blogspot.ca/2013/01/sonnette-dentree.html):他使用一个六引脚微控制器和 64 字节的 RAM 来播放一个音频文件。(法语，[谷歌翻译](http://translate.google.com/translate?sl=fr&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&eotf=1&u=http%3A%2F%2Fpicatout-jd.blogspot.ca%2F2013%2F01%2Fsonnette-dentree.html&act=url)

问题中的微控制器是一个 [PIC10F322](http://www.microchip.com/wwwproducts/Devices.aspx?dDocName=en552977) 。其中一个最小的照片，有足够的 512 条指令的闪存，64 字节的 RAM，以及一大堆其他功能，不应该装进一个像尘埃一样小的包。由于微控制器上没有存储音频数据的空间，Jacques 转向了 64 千字节的 I2C EEPROM。PIC 仅通过两个引脚与 EEPROM 通信，允许它读取音频数据，并通过 PWM 将其再次发送到放大器。这一壮举所需的代码只有 253 条指令，并且只使用了几个字节的 RAM 一个非常小的微控制器所能做的令人印象深刻的展示。