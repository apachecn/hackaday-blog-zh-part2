# 用微控制器接触触摸屏

> 原文：<https://hackaday.com/2012/05/04/reaching-out-to-a-touch-screen-with-a-microcontroller/>

![](img/be634931453c0f5c9542d8e92ec9cf26.png "foil-touchscreen-actuator")

我们喜欢电容式触摸屏。它们比电阻式触摸屏坚固得多，如果用户界面编程良好，它们会产生很好的用户体验。但是让你的电子项目与一个互动有点困难。[RobB]一直在该领域进行实验，并设法为微控制器使用制作了一个简单的触摸屏致动器。

在休息后的视频中，你可以看到他的概念证明。他正在使用 Arduino 每秒一次在 Android iOS 计算器应用程序上输入数字 2。完成这个把戏并不需要太多时间，[RopB]只是在屏幕上贴了一片锡纸，并用跳线将其连接到 Arduino。该引脚保持悬空，直到需要点击屏幕，此时它被拉至地。

运行速度较慢的自定义应用程序可以将此用作输入技术。两片箔片(一片作为时钟，另一片作为数据)将提供一个基本的串行传输系统。

[http://www.youtube.com/watch?v=JDgDMBquBw0](http://www.youtube.com/watch?v=JDgDMBquBw0)