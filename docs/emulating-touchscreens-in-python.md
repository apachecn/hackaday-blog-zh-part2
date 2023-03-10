# 在 Python 中模拟触摸屏

> 原文：<https://hackaday.com/2014/05/18/emulating-touchscreens-in-python/>

![DOS](img/bfabc306abdfba375e62e95e686da039.png)

软件，尤其是用于 CNC 控制的基于 DOS 的软件会永远存在，但硬件肯定不会。当面对用于控制慢慢死去的 CNC 机器的老旧硬件时，[Oliver]需要一种能够模仿 3M Microtouch 触摸屏的东西。不想走硬件路线，他决定用 Python 模拟触摸屏。

Python 代码相当简单，接受鼠标输入并将其翻译成 3M Microtouch 使用的串行协议，因此也是旧的 DOS CNC 应用程序使用的串行协议。然而，编写 Python 来捕捉鼠标点击只是问题的一半。[Oliver]还需要一种方法将这些鼠标点击发送到旧的 DOS 应用程序。虚拟化一台运行 DOS 的旧机器会产生一些时间问题，但最终找到了一个解决方案，使用 DOSBox 和[虚拟串行端口仿真器](http://www.eterlogic.com/Products.VSPE.html)可以连接两个具有串行端口的应用程序。

[奥利弗]终于能够让一切正常工作，让这个设备起死回生，至少再用 30 年。让我们只希望所有的代码都被很好地记录下来，并存档给下一个人。