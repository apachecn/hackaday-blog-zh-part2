# 用旧的吉他英雄踏板控制你的网络摄像头

> 原文：<https://hackaday.com/2012/10/03/controlling-your-webcam-with-an-old-guitar-hero-pedal/>

![](img/d2e80f72283fe522d99617d125460c7b.png "webcam-pedal")

hack aday reader[白梓轩]经常使用 Skype 与远近的家人联系，但他厌倦了每次他的孩子离开画面时调整他的网络摄像头。虽然他提出的解决方案不是全自动的，但它是免提的，这对于他的目的来说已经足够好了。

[Tom]正在四处寻找某种电子脚踏板时，他偶然发现了一个无线第三方吉他英雄外设，恰好符合要求。通过使用由[比尔·波特]创建的[Arduino 库，他很快就能让这个玩具与一个 Arduino 闪存 Atmega8 进行通信，但当需要将信号传回他的电脑时，事情就有些不妙了。使用另一台 Atmega8 和 PS2X 库，他能够模拟他的脚踏板正在寻找的吉他英雄控制器。](http://hackaday.com/2010/06/02/hdsps-and-playstation-2-controllers-on-arduinos/)

随着他的项目的踏板部分结束，他专注于他的网络摄像头。[Tom]将摄像机安装在一个小型伺服系统上，然后连接到他的脚踏装置的接收端。正如你在下面的视频中看到的，他现在可以用脚轻轻一点就能把他的摄像机在房间里平移，而不是靠在地上手动调节。

[https://www.youtube.com/embed/UMS9BExhU1U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UMS9BExhU1U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)