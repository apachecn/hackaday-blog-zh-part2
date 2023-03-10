# 教单词时钟一些新的技巧

> 原文：<https://hackaday.com/2014/07/29/teaching-the-word-clock-some-new-tricks/>

![wordclock2014](img/3fd264b8a920d9dec9920cf62985eb76.png)

[Joakim]制造了一个用文字显示时间的[钟。等待第二字钟，](http://diycrap.blogspot.no/2014/07/wordclock-based-on-arduino-yun.html)[这是什么，2009 年](http://hackaday.com/2009/09/27/word-clock-tell-the-time-with-words/)？[单词钟](http://hackaday.com/2014/07/19/a-laser-cut-word-clock/)是那些已经成为永恒的项目之一。当我们看到一个突出的建筑时，我们一定要把它写下来。【Joakim 的】时钟很特别，原因有很多。时间是用挪威语拼写的，因为这个钟是送给[丹尼尔]的生日礼物，[Joakim]把他的全名~~加到了这个钟的节目单上。~~

字钟设计的难点之一是控制光溢出。[Joakim]使用一个简单的 3D 打印框架来封装每个 LED。这使溢出得到控制，并使一切更容易阅读。使用的 RGB LED[joa Kim]也与标准略有不同。[Joakim]使用的不是 WS2812 Neopixel，而是 LPD8806 LED 灯条。在控制器方面，[Joakim]选择 Arduino Yun 可能有点过火，但他确实很好地利用了 ATmega328 和嵌入式 Linux 机器。

真正的奇迹发生在开机时。[Daniel]的名字以红色亮起，随着每一步的完成，各种字母变为绿色。绿色“D”表示从路由器的 DHCP 服务器获得了 IP 地址。当已经联系了四个 NTP 服务器，并且 Linux 处理器合理地确定它具有正确的时间时，n’切换到绿色。最后一个要更改的字母是“E ”,表示环境光。

[Joakim]增加了一个 web 界面来触发他的新功能，如彩虹调色板，或通过改变字母 K，L，O，K 的颜色来显示分钟的能力。最终的结果是一个光滑的包，这无疑使 2009 年的时代设计达到了 2014 年的标准！