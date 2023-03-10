# 逆向工程一个巨大的 LED 显示屏

> 原文：<https://hackaday.com/2014/08/28/reverse-engineering-a-huge-led-display/>

![muchosLEDs](img/2f04ae03a777f1fe147084aba4357908.png)
在一阵令人敬畏的抢救中，【Piet】拿起一个巨大的，16 字符，2 行显示器。它很大，是为户外设施设计的；路标、火车站等等。当没有任何东西显示时，它还消耗 23 瓦*[的能量，这使得它成为逆向工程](http://devae.re/projects/muchosledjes/)的完美回收设备。*

 *显示器最初连接到运行专有软件的计算机。显示器和计算机之间的协议也是专有的，这让[Piet]可以选择对协议进行逆向工程，或者对硬件进行逆向工程并构建一个新的驱动板。对于任何有烙铁的人来说，第二种选择是最简单的。

拆开显示器，[Piet]发现显示器中的每个字符都是一个 7×14 像素阵列，每个像素阵列有四个 led。每个字符的行和列通过移位寄存器寻址，通过 Arduino，[Peit]使单个字符工作。

Arduino 很难在显示器上显示所有的字符，所以拿出了一个 Raspi，编写了一个驱动程序和帧生成器，整个事情都连接到 Twitter。这是一个漂亮的显示器，扫描像素时消耗 200 瓦，对废弃的硬件进行了奇妙的再利用。下面视频。

[https://www.youtube.com/embed/trRJJdUFywk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/trRJJdUFywk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)*