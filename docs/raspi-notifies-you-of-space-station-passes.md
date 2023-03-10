# 拉斯皮通知你空间站通行证

> 原文：<https://hackaday.com/2013/12/13/raspi-notifies-you-of-space-station-passes/>

![ISS](img/a46a5eebf31add8d558cec66b9a4230f.png)

几个月前，利亚姆在 Kickstarter 上投资了一个小桌面玩具，这个玩具可以告诉他国际空间站何时在头顶上。[利亚姆]有点厌倦了等待，[所以他决定用树莓派和天文计算 Python 库来构建自己的](http://issabove.com/iss-above-and-the-raspberry-pi/)。

这个构建令人印象深刻的部分是根据国际空间站的轨道元素计算轨道物体在天空中的位置。为此，[Liam]正在使用 [PiEphem](http://rhodesmill.org/pyephem/) ，这是一个可以计算太阳、月亮、行星、小行星和地球轨道卫星位置的库，给定位置和时间。由于[号国际空间站的轨道参数](http://www.heavens-above.com/orbit.aspx?satid=25544)经常变化，他的软件被设置为大约每周下载一次更新。

[利亚姆] [开发了他的空间站探测器的几个版本](http://issabove.com/versions/)，每个版本都有不同的显示屏。最简单的使用几个发光二极管，或者通过一个 [LedBorg](http://issabove.com/versions/with-the-ledborg/) 、 [Blinkstick](http://issabove.com/versions/with-the-blinkstick/) ，或者 PiGlow 作为国际空间站在上空时的通知。两个更复杂的版本使用 LCD 显示器或 LED 矩阵来显示下一次 ISS 通过的时间。

下面是视频演示。

[https://www.youtube.com/embed/fAkWuoTsqyk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fAkWuoTsqyk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)