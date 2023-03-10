# Hackaday 奖参赛作品:青少年的绝佳音频

> 原文：<https://hackaday.com/2015/07/26/hackaday-prize-entry-superb-audio-with-the-teensy/>

Raspberry Pi 和 Teensy 3 都有 I2S 接口，这意味着这些板可以用来播放非常高质量的音频。编解码器和 I2S 接口是一回事，但将数字流转换成高质量的模拟输出完全是另一回事。你只需要看看发烧友论坛，就能找到足够的错误和虚假信息来证明这一点。

他的 Hackaday 奖参赛作品是为青少年制作一个音频板。它具有非常高端的运算放大器、合适的滤波器和正确的拓扑结构，可以将数字音频流转换为模拟信号，满足最敏感的耳朵。

Teensy 超级音频板使用 Cirrus CS4272 音频编解码器芯片，这是一种高质量芯片，可以在 24 位深度处理高达 192kHz 的采样速率。这种芯片不包括模拟输入和输出缓冲器，这意味着[威廉]有相当的建设在他面前。这意味着使用[高质量运算放大器](http://www.ti.com/product/ths4521)，低噪声电源，并知道如何构建电路*和测量其噪声*。

到目前为止，测试揭示了这个小电路板令人难以置信的动态范围、平坦度和频率响应。[它也适用于树莓酱](https://hackaday.io/project/5912-teensy-super-audio-board/log/20437-working-with-raspberry-pi)。现在只需要再把这些主板组装起来，就可以获得黑客日奖的[最佳产品](https://hackaday.io/submissions/bestproduct/list)部分了。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)