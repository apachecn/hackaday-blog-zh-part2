# 街头艺术机器人

> 原文：<https://hackaday.com/2013/03/03/street-art-bot/>

[![Street Art Bot](img/beb97a9b224866e2b7529242b01ef633.png)](http://hackaday.com/?attachment_id=95468)

对于解构分散式黑客马拉松，来自塔尔萨 Fab Lab 的“制造者”建造了一个街头艺术机器人。机器人四处行驶，按照一定的模式分配液体粉笔来制作人行道艺术。

制造商的机器人基于电动轮椅平台。附着在底座上的是分发粉笔的硬件，它是通过 wifi 控制的。操作员驾驶机器人在该区域周围进行粉笔绘制，粉笔以正确的图案沉积。

为了确保艺术被正确地记录下来，机器人的软件需要知道机器人一直在哪里。这是通过安装在该区域上方的摄像机和定位机器人的基准标记来完成的。使用[react vision](http://reactivision.sourceforge.net/ "reacTIVision")库完成跟踪。

该机器人是可扩展的，将来他们想添加多种颜色，甚至多个机器人同时打印。休息之后，请观看该项目的视频概述。



[https://www.youtube.com/embed/XM7aHy1gb0o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XM7aHy1gb0o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)