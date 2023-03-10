# 二极管自制编程

> 原文：<https://hackaday.com/2014/06/26/homebrew-programming-with-diodes/>

![diode](img/11ef8e11c9b2ee597542501a68909fb8.png)

二极管矩阵是为最早的电子计算机实现某种只读存储器的第一种方法之一，即使在今天，它们也可以被发现深埋在 ASICs 和其他需要某种形式的一次写入存储器的设备的 IP 中。长久以来，[瑞克]一直想用几百个二极管制作一个只读存储器，现在他终于实现了他的目标。更好的是，他的二极管矩阵电路实际上是功能性的:它是 Atari 2600 的 64 字节 ROM，包含一个极其简单的演示程序。

[Rick]沿着网格连接了一吨 1N60 二极管，对应到 2600 的 CPU 的数据和地址线。在每个交叉点，数据线要么没有连接，要么用二极管连接在一起。如果连接了二极管，将地址线拉高或拉低([Rick]没有公布原理图)会将数据线拉至相同的电压。对每个字节重复这八次，你可能就有了最原始形式的只读存储器。

至于用二极管编码的演示？它显示了一个黑色矩形的彩虹颜色，可以用操纵杆在屏幕上移动。下面视频。

[https://www.youtube.com/embed/LvGyRRIgvjk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LvGyRRIgvjk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)