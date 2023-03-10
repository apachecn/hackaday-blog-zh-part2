# 声纳与 Python 和电话会议硬件

> 原文：<https://hackaday.com/2013/12/23/sonar-with-python-and-conference-call-hardware/>

![conference-call-sonar](img/d6917c9b571ac73c3117e2a421dd77dc.png)

[Jason]刚刚向我们透露了他最近的实验，其中他使用标准音频设备和定制的 Python 程序创建了一个[声纳系统](http://shortcircuitsandinfiniteloops.blogspot.ch/2013/12/new-project-sonar-experiments.html)。如果我们的一些读者还不知道，[声纳](http://en.wikipedia.org/wiki/Sonar)是一种利用声音传播来探测水面上或水面下物体的技术。它通常用于潜艇和船只的导航。[Jason]的项目使用主动声纳，它包括发送短音频脉冲(啁啾声)和倾听回声。回声返回的时间越长，物体就越远。尽管他的概念证明没有在水下使用，但如果他继续这个项目，这种情况可能会改变。

音频编辑软件 [Audacity](http://audacity.sourceforge.net/) 用于制作快速频率变化的啁啾声，以及用于主 Python 程序的 PyAudio 库。通过[将麦克风输出与发射信号相关联](http://en.wikipedia.org/wiki/Cross-correlation)来检测准确的到达时间。鉴于[Jason]使用音频，我们认为下面嵌入的视频中显示的最终结果非常好。

[https://player.vimeo.com/video/82524331](https://player.vimeo.com/video/82524331)