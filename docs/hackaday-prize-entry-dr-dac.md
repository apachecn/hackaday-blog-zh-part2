# Hackaday 奖参赛作品:DAC 博士

> 原文：<https://hackaday.com/2015/06/01/hackaday-prize-entry-dr-dac/>

今年 Hackaday 奖的主题是。建立一些重要的东西。这是一个崇高的目标，但还有第二个奖项，即最佳产品奖，将奖励给一个幸运的团队 10 万美元，这个团队可以吸引那些张着大嘴和钱包的人。这是一个令人难以置信的奖项，其中还包括在 Hackaday 设计实验室的六个月实习，但目前没有多少人争夺 Hackaday 奖的这一部分。

[【drewrisinger】的 DrDAC USB 音频 DAC](https://hackaday.io/project/5996-drdac-usb-audio-dac) 是角逐最佳产品奖的项目之一。他正在解决似乎无处不在的糟糕的低质量内置声卡的问题。是的，这是一个简单的想法，但执行是伟大的。

DrDAC 的电子设备与你所期待的 DIY 音频声卡非常相似；PCM2706 接收 USB 音频并通过 I2S 发送出去。PCM1794 将 I2S 转换为模拟音频，OPA2836 将其放大，并通过 1/8”插孔或一对 RCA 插头发送出去。

[drewrisinger]将 DrDAC 作为学校项目开始，在收到 PCB 后，他注意到一个问题。MultiSim 的 TQFP-32 封装尺寸太小，这意味着 IC 根本不适合电路板。这学期订购新的主板已经太晚了，这意味着需要进行某种返工。[drew]通过在焊盘和芯片引线之间焊接跳线解决了这个问题。是的，这看起来很疯狂，但显然是有效的。你可以在下面看看整个过程的视频。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/nQStPyqFPLY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nQStPyqFPLY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)