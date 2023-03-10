# 协议窥探数字音频

> 原文：<https://hackaday.com/2014/11/12/protocol-snooping-digital-audio/>

越来越多的俱乐部开始数字化。当你出去听一个乐队时，他们正在舞台上插入 ADC(模数转换器)盒，数字化的音频数据通过以太网传输到调音台。这样一来，场地就不必长距离铺设许多音频电缆，但要侵入就困难多了。所以[Michael] [在他的 ProCo Momentum gear 上训练流行的网络分析工具](http://blog.gmichael225.com/post/48khz-adventures)来看看数据是什么样子的。

[Michael]对该过程的描述有点稀疏，但他列出了完成工作所需的所有组件。首先，他使用 Wireshark 查看原始数据。一旦他弄清楚了八个通道是如何分割的，他就使用命令行版本( [tshark](https://www.wireshark.org/docs/man-pages/tshark.html) )和标准的 Unix 命令行工具( [cut](http://www.linuxcommand.org/man_pages/cut1.html) )来分离数据。现在他有了八个声道音频数据的文本表示。

使用 [xxd](http://www.linuxcommand.org/man_pages/xxd1.html) 将数据从文本转换为二进制，然后他使用 [sox](http://sox.sourceforge.net/) 播放它，看看它听起来像什么。还没有骰子。经过一段时间的反复试验，他意识到这些数据是无符号的大端整数。他又试了一次，一切听起来都很好。成功！

虽然这不是一个像[这个](http://hackaday.com/2014/10/30/reverse-engineering-a-blu-ray-drive-for-laser-graffiti/)一样的完整的逆向工程教程，但我们认为它达到了高潮:使用一堆正确的工具和一些好的预感来找出一个晦涩的协议。