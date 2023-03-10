# 利用软件无线电进行实时 GPS 解码

> 原文：<https://hackaday.com/2012/08/19/real-time-gps-decoding-with-software-defined-radio/>

![](img/2d1114d731e68eb6fc186d6cc6159ba2.png "GPS")

如果基于 Realtek RTL2832u 的 USB 电视调谐器加密狗不够有用，那么一个项目背后的人可以让软件定义的 GPS 接收器离开地面[成功地用这个非常便宜的无线电绘制实时 GPS 数据](http://www.gnss-sdr.org/documentation/gnss-sdr-operation-realtek-rtl2832u-usb-dongle-dvb-t-receiver)。

之前，我们已经看到这些软件狗[从 GPS 卫星](http://hackaday.com/2012/04/13/those-usb-tv-tuners-used-for-sdr-can-also-grab-gps-data/)获取数据——如果你正在构建一个基于 GPS 的时钟，这很有用——但这一构建需要数小时的数据收集才能在地图上绘制出你的位置。

GNSS-SDR 项目的工作人员使用 RTL2832 USB 电视调谐器和 Garmin 有源 GPS 天线来实时跟踪多达四颗 GPS 卫星，并绘制精确到约 200 米的位置。

本文的谷歌地球图显示了 GNSS-SDR 团队收集的数据；在整个测试过程中，天线固定在红色箭头处，黄线代表计算位置每 10 秒改变一次。令人惊讶的工作，只是去显示这个非凡的硬件有什么能力。