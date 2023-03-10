# Arduino 数据记录器绘制出你早晨通勤路上的坑洼

> 原文：<https://hackaday.com/2012/11/23/arduino-data-logger-maps-out-the-potholes-on-your-morning-commute/>

![](img/2b71b021224002ab5e00d050ebebfd8f.png "arduino-data-logger-maps-bad-roads")

现在你可以通过测量你的旅程实际上有多崎岖来证明你是办公室里最颠簸的通勤者。[Techbitar]称这个项目为 Bump-O-Meter。它使用 Arduino、GPS 和加速度计来绘制崎岖的道路。

硬件建立在试验板上，[Techbitar]详细介绍了与所用的每个模块的连接和通信。一旦运行，记录器将读取多达六个传感器，并将其记录到 SD 卡中。在休息后的视频中，他展示了用于转储和绘制数据的方法。他从查看电子表格中的数据开始。文件中包含了许多字段，但是只需要其中的三个来绘制上面看到的内容。在缩小了列数后，他转向 [GPS 可视化器](http://www.gpsvisualizer.com/)并上传数据集，该数据集随后被自动绘制在地图上。

在一个乌托邦社会中，所有城市拥有的车辆都会有一个这样的系统，坏的路段会自动出现在道路工作人员的维修清单上。

[https://www.youtube.com/embed/0nOlr9eKyes?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0nOlr9eKyes?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)