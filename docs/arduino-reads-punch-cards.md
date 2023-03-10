# Arduino 读取穿孔卡

> 原文：<https://hackaday.com/2015/01/17/arduino-reads-punch-cards/>

几十年来，穿孔卡一直是程序和数据存储的标准形式，但你今天环顾四周就不会知道了。打卡机甚至阅读器都变得越来越稀少和昂贵。有时需要一点黑客技术 [YouTube 链接]才能让这台旧机器重新运转起来！

[Antiquekid3]设法在 Ebay 上获得了一个旧的穿孔卡片阅读器，但是没有办法与它连接。阅读器原来是一个 Documation M-1000-L，经过一番查找，[Antiquekid3]设法在 [BitSavers](http://bitsavers.trailing-edge.com/) 上找到了[手册](http://bitsavers.trailing-edge.com/pdf/documation/M1000L_TechMan_1971.pdf)【PDF 链接】。事实证明，Documation reader 对每行数据都使用了离散输出。人们可能会认为 Documation 阅读器非常适合隐藏在[古董 3]视频背景中的 PDP-8，但不幸的是，8 缺乏必要的综合卡来与阅读器接口。

[Antiquekid3]毫不畏惧地将一些现代硬件融入其中，并使用 Arduino Uno 作为串行接口的文档。Arduino 有足够的 I/O 来连接读卡器的接口。它还有一个串行接口，使输出数据变得轻而易举。ATmega328 甚至有足够的能力将每张卡从 IBM 的多种键控穿孔格式之一转换成串行格式。

[antiquekid 3]测试卡牌原来是浮点数据集。用电子表格绘制数据会产生一组很好的线性数据点。当然，没有人知道这些数据意味着什么！想要更多的打孔卡吗？看看这个 [tweeting punch card reader](http://hackaday.com/2014/11/21/tweet-messages-from-punch-cards/) ，或者这个[基于 Arduino 的阅读器](http://hackaday.com/2012/07/30/reading-punch-cards-with-an-arduino-and-digital-camera/)，它使用乐高和数码相机来哄纸数据。

[https://www.youtube.com/embed/N27Mr199I7g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/N27Mr199I7g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)