# 嗅探 PH 传感器射频信号以获得反馈:您的食道

> 原文：<https://hackaday.com/2014/03/31/sniffing-ph-sensor-rf-signals-for-feedback-re-your-esophagus/>

大约一个星期以来，[贾斯汀]在他的食道里装了一个无线酸度传感器，在他的口袋里装了一个看起来像寻呼机的射频接收器。所以他很自然地决定使用 RTL-SDR 加密狗来[嗅出他发出的信号](http://dolske.wordpress.com/2014/03/25/hacks-all-the-way-down/)。正如我们大多数 Hackaday 读者所知，这些基于 RTL2382U 的廉价 DVB-T 接收机在收听 50MHz 至 1800MHz 之间的任何内容时都非常方便。[Justin]实际上在列出这些接收器的所有用途方面做得很好(飞机交通监控、天气图像下载、电表读数、起搏器监控……)。

经过一些谷歌搜索后，他设法找到了他的 Bravo pH 传感器用户指南，因此发现了它的主要频率和调制方案(433.92MHz / ASK)。[Justin]然后使用 [gqrx](http://gqrx.dk/) 和 Audacity 手动解码数据包，然后编写一个使用音频文件的基于浏览器的工具。最后，几个小时的额外思考让他能够提取他亲爱的食道的 pH 值。