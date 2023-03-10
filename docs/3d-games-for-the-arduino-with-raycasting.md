# 支持光线投射的 Arduino 游戏

> 原文：<https://hackaday.com/2012/09/09/3d-games-for-the-arduino-with-raycasting/>

![](img/85fe7d43f77caf4f6e34fd2e2ae9168b.png "ray")

对于我们看到的所有基于 Arduino 的视频游戏版本，我们实际上只剩下一堆 2D 平台和其他基于 sprite 的游戏。[赖梅克]并不满足于这种程度的计算复杂性，所以他[将由*杜克·纽肯 3D* 制造的 3D 游戏引擎移植到 Arduino](http://arduino.r-bau.de/index.php?page=4&obj=26) (德语，[谷歌翻译](http://translate.google.com/translate?sl=de&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Farduino.r-bau.de%2Findex.php%3Fpage%3D4%26obj%3D26&act=url))上。

[Reimecker]的项目是基于由[Ken Silverman]编写的非常受欢迎的[构建引擎](http://advsys.net/ken/build.htm)，并在游戏中使用，如*杜克 Nukem 3D*、*暗影战士*、*热血、*和 *TekWar* **。** 构建引擎可以用来制作第一人称射击游戏，但更多的是在 *Wolfenstein 3D* 而不是*半衰期的层面上。*

使用的硬件[Reimecker]是一个常规的 8 位 Arduino，带有一个附加的 LCD 触摸屏，显示 320×240 像素的光线投射环境。从这个版本的视频来看(休息之后可以看到)，[Reimecker]有一个相当不错的游戏引擎，能够显示 2.5D 的环境。帧速率可能不是很高，但考虑到[Reimecker]正在使用的硬件，这仍然是一个惊人的构建。

[https://www.youtube.com/embed/BxW5ZtcXx0E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BxW5ZtcXx0E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/WJi85lr5Ofo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WJi85lr5Ofo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/9M32PF1IVQg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9M32PF1IVQg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/iE8F2E5CnCI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iE8F2E5CnCI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)