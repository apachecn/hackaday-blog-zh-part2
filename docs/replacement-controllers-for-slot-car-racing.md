# 老虎机赛车的替换控制器

> 原文：<https://hackaday.com/2013/01/23/replacement-controllers-for-slot-car-racing/>

![replacement-controllers-for-slot-car-racing](img/c6dfc88c03f088fc24c57babd579e8cf.png)

右边的模糊部分是一辆冲进画面的汽车。但是环顾图像的其余部分，您会发现该区域散落着额外的硬件。[Matthew]、[Doug]和[Barry]一直在努力工作[在这个 Scalextric 老虎机设置上添加额外的功能并替换原有的控制器](http://code.google.com/p/turbo-scalextric/)。到目前为止，看起来他们的构建日志还没有赶上他们已经完成的所有工作。我们希望了解更多的细节，因为他们有时间写这些(这是大学的课程，所以我们肯定他们有很多事情要做)。但是现在有几个视频和[一个图片库](https://picasaweb.google.com/106450760778238715474/TurboScalextric?authuser=0&feat=directlink)让人垂涎欲滴。

赛车由赛道上的电压控制。团队用覆盆子酱代替了库存控制器。它通过 MOSFETs 使用脉宽调制来管理该电压。这使得比赛可以自动化，同时也使得人类操作员可以简单地使用任何可以想象的输入设备来控制赛车。为了更好地测量，他们还增加了一个计圈器，使用红外 LED 和探测器来感应赛车何时通过终点线。

在看了他们的几个视频后，我们认为这个项目的目标是记录最快的时间，而不是让赛车在转弯时飞出赛道。