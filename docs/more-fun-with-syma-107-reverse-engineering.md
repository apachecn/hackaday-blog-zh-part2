# 司马 107 逆向工程更好玩

> 原文：<https://hackaday.com/2012/12/08/more-fun-with-syma-107-reverse-engineering/>

[![Syma Reverse Engineering](img/a26843dce42183648dd3b422fbe7434c.png)](http://hackaday.com/2012/12/08/more-fun-with-syma-107-reverse-engineering/symareverse/)

[Jim]使用逻辑分析仪对 Syma 107G 直升机的红外协议进行了深入分析。我们在过去的中已经看到了对这个协议[进行逆向工程的工作，但是【吉姆】已经对它进行了改进。](http://hackaday.com/2012/08/27/reverse-engineering-a-syma-107-toy-helicopter-ir-protocol/ "Reverse engineering a Syma 107 toy helicopter IR protocol")

[Jim]没有读取控制器的 IR 输出，而是将一个[salae 逻辑](http://www.saleae.com/logic "Saleae Logic")直接连接到控制器的电路上。这使他能够获得更准确的时间，这有助于他发现一些关于该协议的新东西。他用这个创建了一个协议的详细解释。

一个主要的发现是控制器使用了一个 3 字节的控制包，这与过去对设备的逆向工程相矛盾。对于多通道的工作原理也有了新的解释。这使得多架直升机可以在没有控制人员干扰的情况下飞行。

这篇文章非常详细，解释了逆向工程的过程。它还为任何想黑掉这些低成本直升机的人提供了很好的信息。从[Jim]制定的细节来看，在您自己的硬件上实现该协议是相当容易的。