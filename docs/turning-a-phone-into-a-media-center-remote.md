# 将手机变成媒体中心遥控器

> 原文：<https://hackaday.com/2013/05/20/turning-a-phone-into-a-media-center-remote/>

![IMG_2061](img/0de012b579ffab44cbefcad698534355.png)

[Kees]想要一个 XBMC 音响系统的遥控器。他在他的一个项目箱中放了一部经典的 T65 荷兰电话，他认为这部电话加上树莓皮后，他[可以拥有一个功能性的媒体遥控器](http://www.keesvanweert.nl/blog/?p=1)，具有经典的线条和 70 年代的风格。

电话上的每个数字都被连接到一个小的无焊试验板上。用几个电阻，[Kees]建立了一个简单的上拉/下拉电路，馈入他的 Raspi 的 GPIO 输入。

通过一个简短的 Python 脚本，[Kees]成功地将按钮映射到 XMBC 的播放/暂停、音量增大/减小、下一个和上一个命令。还剩下一些按钮，所以这些按钮被映射到在线电台、播放列表和一个只被称为“moo”的奇怪设置。我们不确定这个按钮是做什么的，但是你可以在下面的视频中看到这个 XMBC 电话遥控器的其他功能。

[https://www.youtube.com/embed/MZjX6UAjFxQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MZjX6UAjFxQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)