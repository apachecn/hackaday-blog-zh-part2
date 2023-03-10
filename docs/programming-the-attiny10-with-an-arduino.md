# 使用 Arduino 对 ATtiny10 进行编程

> 原文：<https://hackaday.com/2012/08/23/programming-the-attiny10-with-an-arduino/>

ATtiny10 以及它的兄弟姐妹 ATtiny 4、5 和 9 是 Atmel 制造的最小的微控制器。尽管只有 32 个字节的 RAM 和 1 kB 的闪存，你仍然可以用这个小小的 6 针芯片做很多事情。[费曼 17]想出了一个用 Arduino 给这个芯片[编程的方法，允许他对这个小得离谱的微控制器扔任何东西。](http://junkplusarduino.blogspot.jp/p/attiny10-resources.html)

ATtiny10 没有使用其他基于 Atmel 的主板上常见的 ISP 编程头。相反，它使用非常奇怪的[微型编程接口](http://www.atmel.cimg/doc8373.pdf)将位写入芯片上的闪存。[feynman17]意识到他可以使用 Arduino SPI 库与该芯片进行通信，并利用几个电阻和一个 8 引脚 DIP 插座构建了一个小型编程屏蔽，以安装 ATtiny10 分线板。

在完成了从 Arduino 串行控制台上传一个. hex 文件的草图之后，[费曼]就有了一个编程的 ATtiny10，随时可以投入到他脑海中任何一个惊人的小项目中。

至于你可以用这个小微控制器做什么，芯片调谐永远是一个选项，就像让 T2 成为一个非常非常小的西蒙克隆体一样。它可能不是一个动力室，但你仍然可以用这个非常便宜的微控制器做很多事情。