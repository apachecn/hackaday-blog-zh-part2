# 我们向电视管旗致敬

> 原文：<https://hackaday.com/2014/02/24/we-salute-the-television-tube-flag/>

从[Gijs]而来的是 [Beeldbuis Vlag Tijsdlijn，即电视显像管](http://gieskes.nl/undefined/STRPsenior/BV/tijdlijn.html)旗([译为](http://translate.google.com/translate?hl=en&sl=nl&tl=en&u=http%3A%2F%2Fgieskes.nl%2Fundefined%2FSTRPsenior%2FBV%2Ftijdlijn.html))。我们还不了解我们的荷兰人，但是看起来[Gijs]和他的朋友们已经发明了一种电视显像管，这种显像管在风扇气流的作用下会像旗子一样飘动。这种效果是相当惊人的，这是温和的说法。为了创造这个黑客，[Gijs]建造了一个改良的[摆动器](http://vimeo.com/16906546)。摆动器是一个早期的视频合成器，它使用附加的转向线圈来修改标准电视显像管的操作。当受到激励时，线圈会使电子管的电子束偏转，从而在屏幕上出现一些相当模糊的图像。(是的，在 hack aday,“trippy”是一个科学术语。

[Gijs]希望他的屏幕被粉丝“挥动”,就像旗帜会挥动一样。为此，他使用了由乒乓球两半组成的风速计。风速计通过光盘驱动旋转 DC 马达。在这种应用中，电机充当发电机，产生 DC 电压。运行 Arduino 代码的 ATmega328 从电机读取电压。如果风速计在旋转，Arduino 会输出一个正弦值。Arduino 的输出被放大并应用于 CRT 上的线圈。功率电阻网络确保放大器负载正确。结果不言自明。在休息后的视频中，地铁旗帜正在展示其建设的照片幻灯片。作为一个额外的黑客，[Gijs]使用 Arduino Leonardo 作为 USB 键盘。当风速计旋转时，主 ATmega328 向 Leonardo 发送信号，然后 Leonardo 模仿主机上箭头键的按下。这让管旗推进自己的形象。非常酷的作品！

[https://www.youtube.com/embed/R55T4y-i6jQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/R55T4y-i6jQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)