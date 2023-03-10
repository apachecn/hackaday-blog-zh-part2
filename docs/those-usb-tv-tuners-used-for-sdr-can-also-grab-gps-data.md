# 那些用于 SDR 的 USB 电视调谐器也可以抓取 GPS 数据

> 原文：<https://hackaday.com/2012/04/13/those-usb-tv-tuners-used-for-sdr-can-also-grab-gps-data/>

![](img/efacf1ae0eb0b744e7570b4115eef609.png "usb-tv-tuner-as-gps-module")

谈谈多功能硬件。这些便宜的电视调谐器适配器也可以获取 GPS 数据。你可能还记得看到同样的硬件[被用作软件定义无线电](http://hackaday.com/2012/03/30/working-software-defined-radio-with-a-tv-tuner-card/)的 20 美元选项。但是(米歇尔·巴瓦罗)决定看看他们还能耍出什么花招。

他能得到精确到 20 厘米的位置数据，你会感到惊讶吗？这个数字并不能说明全部情况，因为读数是在电子狗静止三个小时后获取的，然后进行平均以达到这种精度。但是根据你的需要，这方面的数据可能不成问题。[Michele]确实计划在他的下一个项目中实现实时 GPS 数据。他计划使用 SDR 采集算法来测量多普勒频移，以解释与标准 GPS 接收器相比，软件狗的时钟速度较慢。我们可以理解这将如何工作，但我们很高兴他有能力实际实现它，因为我们不知道如何实现这个概念。

[via [Reddit](http://www.reddit.com/r/gadgets/comments/s7ekz/remember_that_project_to_turn_20_tv_tuners_into)