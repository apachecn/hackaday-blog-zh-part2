# 用 Raspberry Pi 构建的自动化编程和测试夹具

> 原文：<https://hackaday.com/2013/06/10/automated-programming-and-testing-jig-built-with-raspberry-pi/>

[道格·杰克逊]做文字钟，他一定做了不少生意。我们这么说是因为他为时钟电路板组装了一个[编程和测试平台。](http://www.instructables.com/id/A-Programming-Jig-for-our-DougsWordClockcom-DeskC)

如果您正在进行任何类型的卷组装，这是一个很好的例子。夹具让组装好的 PCB 卡入到位，完成所有必要的电气连接。这是通过他在易贝挑选的一包货物实现的，其中包括将电路板与丙烯酸安装板分开的橡胶垫片、用于进行电气连接的弹簧针，以及图中左侧的弹簧板夹。

右下角的开关将电源连接到电路板，并将 Raspberry Pi GPIO 引脚拉高。运行在 RPi 上的 Python 脚本轮询该引脚，执行 bash 脚本，该脚本使用 AVRdude 的 GPIO 版本对 ATmega169 微控制器[进行编程。我们浏览了他的 Python 脚本，没有看到测试电路板的代码。但是上面的图片在屏幕上显示了一条“通过”的信息，而这并不在他的脚本中。我们敢打赌，他有另一个版本，采取硬件通过自我测试程序。](http://blog.stevemarple.co.uk/2013/03/how-to-use-gpio-version-of-avrdude-on.html)

我们第一次看到道格的单词钟是在 2009 年的时候[，然后几个月后又看到了](http://hackaday.com/2009/09/27/word-clock-tell-the-time-with-words/)。时钟的外观很棒，很高兴看到这个项目仍在强劲发展。