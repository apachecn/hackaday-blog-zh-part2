# 使用 RGB LED 矩阵监控 GitHub 活动

> 原文：<https://hackaday.com/2013/10/16/monitor-github-activity-with-an-rgb-led-matrix/>

![tim-display](img/0b1233cb7643aebbc98848d0bdd39e33.png)

有没有想过是谁在派生你的代码？[Jack]做到了，所以他为他公司的仓库建立了一个[实时 GitHub 活动显示。该显示器基于一个](http://jack.minardi.org/projects/displaying-realtime-github-activity-on-a-full-color-led-matrix/)[智能矩阵(TiM)板](http://www.seeedstudio.com/depot/tim-p-1516.html)。TiM 是普遍存在的 ws 2811/智能像素/新像素 RGB LEDs 的 8 x 16 矩阵，带有内置控制器。随着价格的下降，我们看到越来越多的这种系列发光二极管。焊接跳线允许 TiM 用作 8 个并行的 led 行(为了更高的刷新率)，或者连接成一个长的串行链。

[Jack]并不担心速度，所以他将他的电路板配置成一串发光二极管。Arduino 用一个引脚驱动整个矩阵。与其重新发明轮子，[杰克]不如使用 [Adafruit 的 NeoMatrix 库](http://learn.adafruit.com/adafruit-neopixel-uberguide/neomatrix-library)来驱动他的显示器。由于 TiM 使用与 Adafruit NeoPixel 矩阵相同的 led，该库将正常工作。为开源硬件和软件赢得又一次胜利！

一个电动 Imp 通过 WiFi 检索 Github 数据，并将其传递给 Arduino。这是微控制器的一个很好的用途，例如 Arduino 上的 AVR。[杰克的]显示器有一个滚动的用户名。滚动动画中的每一步都需要将所有像素数据输出到 TiM 板。Arduino 可以处理这些，而 IMP 负责更高级别的任务。

GitHub 动作由形成显示背景的彩色像素表示。最后一个接触存储库的用户的用户名在显示屏上滚动。如果没有某种关键点，很难将背景矩阵颜色转换成活动。我们猜测这将成为展示使用几天后的第二天性。我们不知道[Jack 的]公司是否做任何自动化构建测试，但我们希望看到他的项目与[这个交通灯构建监视器](http://hackaday.com/2012/02/12/monitoring-software-builds-with-a-traffic-light/)合并。一个大的亮红色 LED 矩阵和一个白色滚动的用户名将不会留下任何疑问，谁破坏了这个构建，谁将会工作到很晚来修复它！

[https://www.youtube.com/embed/zrsNJpTwHrw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zrsNJpTwHrw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)