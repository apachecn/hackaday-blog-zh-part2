# 软件定义无线电入门

> 原文：<https://hackaday.com/2012/06/27/getting-started-with-software-defined-radio/>

在过去的几个月里，软件定义无线电的流行程度出现了爆炸式增长，这要归功于一种小型 USB 电视调谐器加密狗，它能够接收 64 到 1700 MHz 之间的任何广播。这是一个非常好的项目，它开启了一系列无线电实验的大门，但在 SDR 世界中起步可能有点令人生畏。为了帮助大家，[MS3FGX]正在[编写入门指南](http://www.thepowerbase.com/2012/06/getting-started-with-rtl-sdr/)，这样每个人都可以进入软件定义无线电的世界。

在获得 RTL-SDR 项目支持的一个电视调谐器(目前最常用的是 Dealextreme 的[这个](http://dx.com/p/mini-dvb-t-digital-tv-usb-2-0-dongle-with-fm-dab-remote-controller-92096?utm_rid=58964868&utm_source=affiliate))之后，接下来你需要的是一个像样的天线。[MS3FGX]在[这个无线电窝棚天线](http://www.radioshack.com/product/index.jsp?productId=2103077)上取得了一些成功，但[自己制作](http://hackaday.com/2012/05/14/improving-a-software-defined-radio-with-a-few-bits-of-wire/)非常容易。

与 RTL 电视加密狗一起使用的最受欢迎的软件包是[GNU Radio](http://gnuradio.org),【ms 3 fgx】详细介绍了[设置这个](http://www.thepowerbase.com/2012/06/getting-started-with-rtl-sdr/2/)的来龙去脉，并简要介绍了 [Gqrx 接收器](http://www.oz9aec.net/index.php/gnu-radio/gqrx-sdr)。

安装好硬件和软件后，剩下唯一要做的事情就是调到几个你喜欢的电台。RTL 覆盖的频率范围包括 AM 和 FM 无线电，以及 GSM 和 GPS 信号。当然，在这个项目中你还可以做更多的事情，比如监听你汽车上的无钥匙遥控钥匙、寻呼机和无线气象站。