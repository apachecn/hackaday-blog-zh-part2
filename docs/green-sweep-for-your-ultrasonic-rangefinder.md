# 绿色扫描你的超声波测距仪

> 原文：<https://hackaday.com/2014/12/22/green-sweep-for-your-ultrasonic-rangefinder/>

也许你以前从未编写过 Arduino。或者你有，但是除了闪光灯之外没有别的。也许你的烙铁坐在你车库的一个角落里，每次你走过的时候，它都会责备地盯着你，就像一个乞求被扔出去的球。也许你已经做了一些漂亮的项目，但是从来没有把它们和电脑连接起来。如果这描述了你，那么这篇文章和项目正是你所需要的。所以，拿起你最喜欢的饮料，大吃一顿，准备好获得动力。

[Anuj Dutt]不仅做了一个非常酷的项目，他在记录方面也做得非常出色。这是一个类似 project 的 Arduino 控制的“雷达”,它使用了我们熟悉的视差超声波传感器。它被安装在一个伺服系统上，并将数据传送到一台个人电脑上，在那里一个定制的 VB.NET 程序将数据转换到一个很酷的“绿色雷达扫描”屏幕上。它还将文本推送到 LCD 上，显示与目标的距离。

![screenshot of radar program](img/f5b356862b95acf8d8948822c0bc1cb4.png)

[Anuj Dutt]手动滚动他的 Arduino *只是因为*，但是在让一切与 PC 对话时遇到了一些麻烦。他最终使用了超级用户友好的 FTDI 来挽救局面。一定要看看下面的视频，看看这个项目是如何运作的。[Anuj]在视频描述中公布了[Arduino 和 PC](https://independent.academia.edu/AnujDutt/Papers) 的代码。

[https://www.youtube.com/embed/JMDjhuXL5aQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent&listType=playlist&list=UUe-l29Y0-fLyXpkopyHa9JQ](https://www.youtube.com/embed/JMDjhuXL5aQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent&listType=playlist&list=UUe-l29Y0-fLyXpkopyHa9JQ)