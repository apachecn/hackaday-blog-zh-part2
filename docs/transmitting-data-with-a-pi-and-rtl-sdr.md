# 使用 Pi 和 RTL-SDR 传输数据

> 原文：<https://hackaday.com/2013/11/09/transmitting-data-with-a-pi-and-rtl-sdr/>

有时候，最好的构建并不是什么新东西，而是结合了两种成熟的技巧。[Marc]熟悉 RTL-SDR，这款 30 美元的 USB 电视调谐器是软件定义的无线电，但令人惊讶的是，还没有人将这款廉价的无线电加密狗与从 Raspberry Pi 传输无线电的能力结合起来。[【Marc】将这两个版本](http://www.kprod.eu/blog/?p=26)结合起来，为 Raspberry Pi 设计出了最便宜的便携式无线电调制解调器。

把 Raspi 变成一个发射器[其实并没有那么难](http://hackaday.com/2012/12/10/transmit-fm-using-raspberry-pi-and-no-additional-hardware/)；它只需要将一根 20 厘米长的电线插入 GPIO 引脚，然后以大约 100 MHz 的频率切换该引脚。由此产生的信号可以在 50 米外被接收到，甚至可以穿透墙壁。

[Marc]将这个无线电发射机与 [minimodem](http://www.whence.com/minimodem/) 结合起来，minimodem 是一个以所需波特率生成音频调制解调器音调的程序。数据被编码在这个音频流中，通过无线发送，并使用 RTL-SDR 加密狗再次解码。

这本身并不是什么新鲜事，但是如果你正在寻找一个在电脑和 Raspberry Pi 之间的短程、低带宽无线连接，这无疑是最简单和最便宜的方法。