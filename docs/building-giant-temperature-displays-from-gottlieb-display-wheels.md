# 用戈特利布显示轮建造巨型温度显示器

> 原文：<https://hackaday.com/2012/05/07/building-giant-temperature-displays-from-gottlieb-display-wheels/>

![](img/a67f13186aedd48e2841b2ba3907c028.png "Screen Shot 2012-05-04 at 2.48.01 PM")

周六，我们发现了一篇很酷的文章，其中弹球机显示轮被用作显示器。在那篇文章中，列出的灵感之一是这个[巨大的戈特利布轮被用来显示游泳池的水温](http://www.elektor.com/magazines/2012/april/thermometer-using-giant-gottlieb-displays.2114766.lynkx?tab=2)。在我们继续之前，我们想提一下，这个项目是在一个杂志的网站上托管的，需要您注册才能获得 1 个免费下载。我们做了，不需要任何财务信息。

该项目的作者[Ludovic]正在寻找一种高效且高度可视的方法来显示游泳池的温度。他想要一种他能从 30 码外看到的东西，这种东西耗电最少。这些弹球卷轴非常完美，易于阅读，不更新时几乎不耗电。

请继续阅读视频和更多信息。

[https://www.youtube.com/embed/wb8-KjaeI6Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wb8-KjaeI6Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这个项目中的大脑是一个 ATTin2313。整个装置每 20 分钟通电一次，以检查温度。如果温度没有变化，它会重新断电。如果有，它会更新显示。一个 1 法拉的电容器足以让 ATTiny 在作业之间保持活动，以便它可以再次运行该过程。

可下载的 PDF 文档非常深入地解释了该项目的理论、构造和运行，包括完整的原理图和一些有用的资源。