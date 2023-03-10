# 用图表记录器打印文本

> 原文：<https://hackaday.com/2014/07/20/printing-text-with-a-chart-recorder/>

[![A chart recorder printing 'Hello World'](img/341585307b184f71bedf9fc53701fca3.png)](http://hackaday.com/2014/07/20/printing-text-with-a-chart-recorder/chart-recorder/)

图表记录器是用来在纸上绘制模拟值的老式设备。它们类似于从地震中记录地震波的老式地震仪。该设备有一支加热笔，可以在一张热敏纸上移动。这张纸以特定的速度通过机器，它给出了二维绘图。

[Marv]最终得到了几个停产的图表记录器，并找出了接口。五个并行信号控制纸张的进给速度，一个模拟电压控制笔的位置。下一步是连接一个 Arduino 来控制绘图仪。

然而，一旦该设备可以绘制模拟值，[Marv]很快就开始寻找新的挑战。他想用这个设备写字符和位图，但是这需要不连续的线条。通过增加一个螺线管来提升笔，他建造了一个[图表记录器打印机](http://emgoz.blogspot.de/2014/07/a-chart-recorder-printing-text.html)。

休息之后，看看图表记录器做一些它从未打算做的事情的视频。如果你碰巧有一个这样的图表记录器，[Marv]在他的文章中包含了所有的代码，可以帮助你构建自己的图表记录器。

[https://www.youtube.com/embed/QOoc2y8F-bU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QOoc2y8F-bU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)