# Ti Chronos 手表控制树莓 Pi

> 原文：<https://hackaday.com/2012/07/03/ti-chronos-watch-controls-raspberry-pi/>

![](img/15830ae085121147e0732399a6d95319.png "ti-watch-controlled-raspberry-pi")

[Mike Field]正在将他的 TI Chronos eZ430 手表与 Raspberry Pi 连接起来。当事情进行得相当顺利时，他偏离了他的计划,[为 RPi 音频播放器](http://hamsterworks.co.nz/mediawiki/index.php/Watch_Audio)实现了基于手表的控制。

这一点也不奇怪，这是可能的，甚至很容易。毕竟，RPi 板具有原生 USB 功能，可以托管手表的 RF 加密狗，并且它运行的是 Linux，我们知道 Linux 已经可以很好地与 Chronos 平台配合使用。但是我们仍然喜欢把自动化控制绑在手腕上的想法！

mpg321 是这个黑客使用的音频播放程序。它使用 ALSA 播放 MP3 文件，在 RPi 上有一些小问题。[Mike]找到了变通方法，并将它们包含在 C 程序中，他使用 C 程序将所有内容收集到一个漂亮的代码包中。控制依赖于从手表发送的按键(用于 PowerPoint ),这些按键由他的代码翻译并推送到音频/mp3 程序。