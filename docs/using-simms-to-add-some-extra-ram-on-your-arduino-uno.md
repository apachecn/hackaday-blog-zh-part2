# 使用 SIMMs 在 Arduino UNO 上添加一些额外的内存

> 原文：<https://hackaday.com/2014/04/09/using-simms-to-add-some-extra-ram-on-your-arduino-uno/>

单列直插式内存模块(SIMM)是一种包含随机存取存储器(RAM)的内存模块，从 20 世纪 80 年代早期到 90 年代晚期用于计算机(想想 386、486、Macintoshs、Atari STE…)。[Rafael]刚刚做了一个小小的库,允许你将这些模块连接到基于 Atmega328p 的 Arduino UNO，以便获得一些内存空间。他的工作实际上是基于来自[Dmitry Grinberg]的 8 位 atmega 168hack 上的伟大的[Linux，但是需要一些调整来使它与[Rapfael]的 SIMM 一起工作，而且还要将其移植到 Arduino 平台。上面显示的 30 针 SIMM 能够存储高达(抓紧你的椅子……)16MB，但由于 Atmega328p 上可用的 io 数量有限，只能使用 256KB。我们猜测 SPI / I2C IO 扩展器可以解除这一限制。在休息之后嵌入快速(抖动)视频。](http://dmitry.gr/index.php?r=05.Projects&proj=07.%20Linux%20on%208bit)

[https://www.youtube.com/embed/Yah3ViEggxA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Yah3ViEggxA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)