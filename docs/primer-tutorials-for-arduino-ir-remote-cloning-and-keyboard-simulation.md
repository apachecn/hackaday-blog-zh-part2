# Arduino IR 远程克隆和键盘模拟初级教程

> 原文：<https://hackaday.com/2013/11/20/primer-tutorials-for-arduino-ir-remote-cloning-and-keyboard-simulation/>

我们已经展示了大量的 IR Arduino 项目，它们都是令人兴奋和独特的。该项目源于特定的需求或问题，定制的红外遥控器是解决方案。我们在本文中分享的[Rick 的]双重功能也不例外，但[Rick 的]项目有趣和不同的是他仔细和深思熟虑的教程交付，介绍如何复制红外遥控代码，以 Arduino 的风格存储代码，然后发送或接收代码以控制设备。

在他的空间加热器的情况下，Arduino 被用来记录并在他在寒冷的早晨醒来之前向加热器重新发送“通电”IR 代码。这样，在他不得不从被子下爬出来之前，他的房间是温暖的，这有一个额外的好处，可以节省整夜运行加热器的成本。如果你没有可编程的加热系统，这是个好主意。也许有一天他会添加一个温度传感器，这样它就不必严格按照时间运行了。

更复杂的问题是[远程控制他电脑上的 DVD 播放软件](http://www.richardosgood.com/blog/2013/11/19/remote-control-your-computer-using-arduino/)。[Rick]说他坐在远处用电脑看 DVD，但是他的电脑没有像普通电视那样的遥控器。Arduino 又来救援了！但这次他拿出了一个 Teensyduino，因为它增加了能够模拟键盘的功能，当然计算机 DVD 播放软件接受键盘命令。他再次使用“IRremote.h”库来记录旧遥控器上的某些按钮代码，然后将检索到的代码添加到 Teensyduino 设置中，并编程为接收和解码遥控器的红外信号。然后，Teensyduino 将 IR 代码映射到已知的键盘快捷键，并通过其 USB 电缆将模拟的键盘快捷键命令传输到计算机，DVD 播放软件将在此识别键盘命令。

一如既往，[Rick]在他的博客上分享他所有的库和草图，所以请点击上面的链接下载文件。如果你跟随他下面的精彩视频，你不会错过任何一步。另外，这里有一些其他的方法和工具可以让[用你的 Arduino](http://hackaday.com/2012/07/23/using-an-ir-remote-with-your-arduino/) 和[克隆一个红外遥控器](http://hackaday.com/2013/09/15/cloning-an-infrared-disarming-remote-of-a-8-home-security-system/)来使用红外遥控器。

[https://www.youtube.com/embed/jiDnvEzuDCM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jiDnvEzuDCM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/zwnt5SmBFQk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zwnt5SmBFQk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)