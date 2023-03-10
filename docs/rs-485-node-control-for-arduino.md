# Arduino 的 RS-485 节点控制

> 原文：<https://hackaday.com/2012/12/04/rs-485-node-control-for-arduino/>

![rs-485-arduino-nodes](img/9321fada145b214ccf9bcfcb0a5243b1.png)

想要控制一个不在电脑附近的分体式翻盖显示器[Tom]寻求一种通用的远距离通信解决方案，这对于 I2C 或 SPI 来说不切实际。他使用 RS-485 协议开发了自己的硬件和数据包格式。

这是他一直在从事的一个更大项目的一部分，该项目将数据输入到他计划挂在墙上的分体式翻盖显示器中。 [RS-485](http://en.wikipedia.org/wiki/RS-485) 设计用于长距离工作并克服噪音问题。通信系统的核心是[左边看到的电路板](http://unknowndomain.co.uk/blog/2012/08/10/circuitry/)。它使用一个 MAX1483 芯片，一对用于以太网电缆的 RJ45 插孔，以及两个用于电源和通信的端子板。这有一些好的方面。该板作为一个通道，可以很容易地将节点链接在一起，并且数据结构完全独立于硬件本身。因此[Tom]开发了他自己的数据包格式，比我们前几天看到的 [Arduino 网络方案](http://hackaday.com/2012/12/03/inventing-networking-protocols-for-dozens-of-arduinos/)更有弹性。