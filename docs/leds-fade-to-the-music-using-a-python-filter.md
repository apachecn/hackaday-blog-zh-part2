# 使用 Python 滤镜，led 随着音乐渐隐

> 原文：<https://hackaday.com/2012/10/25/leds-fade-to-the-music-using-a-python-filter/>

![](img/f612096e0209a747c67a7f25bc9c79ee.png "using-python-to-pulse-to-the-music")

这个小小的 LED 灯随着音乐逐渐消失。硬件本身非常简单，一些 led 连接到 Arduino 的 PWM 引脚。但是[信号处理是在使用 Python 脚本](http://www.zolmeister.com/2012/10/back-light-music-leds.html)的计算机上进行的。

我们看到的很多项目都是哪些脉冲灯来音乐[使用 MSGEQ7 芯片对音频信号进行硬件处理](http://hackaday.com/2012/09/11/disco-planet-a-massive-rgbw-led-array-in-a-6-globe/)。但由于[佐尔梅斯特]用电脑来演奏他的曲子，他走了一条不同的路线。他的 Linux 盒子使用 PulseAudio 来处理声音。这允许他从音频回放中进行记录，这为 pyAudio 包提供了内部源。他的 Python 脚本将流媒体音频的片段保存到。wav 文件。然后，我将音量标准化，并在删除样本并进入下一个样本之前，使用振幅来设置 PWM 值。这些值以 115200 波特的速率被推送到 Arduino，以实现中断后在视频中看到的结果。

[https://www.youtube.com/embed/V7WKf7O7V5E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/V7WKf7O7V5E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)