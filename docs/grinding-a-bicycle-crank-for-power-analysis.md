# 磨削自行车曲柄进行功率分析

> 原文：<https://hackaday.com/2015/01/11/grinding-a-bicycle-crank-for-power-analysis/>

为了[Mark]和[Brian]在康奈尔大学[Bruce Land]儿童早教课上的最终项目，他们决定复制一个商业产品。这是自行车的仪表板，显示距离、节奏、速度和骑车人产生的能量。计算距离、节奏和速度相当容易，但计算能力完全是另一回事。

这些人正在使用 ATMega1284 驱动 LCD，监听一些霍尔效应传感器，并进行一些计算。它负责测量除了能量之外的所有东西。快速搜索一下[相关的知识产权](https://www.google.com/patents/US7806006?dq=bike+power+meter&ei=CIKGVImOJs-dyATNuoEQ)就有了在踏板曲柄处测量扭矩的想法。为此，[Mark]和[Brian]在一个踏板曲柄上使用了一个应变仪，经过精心修改，使其足够坚硬，可以工作，但又足够灵活，可以测量。

为踏板曲柄构建了一个定制板，用于测量应变仪，并通过无线连接将测量结果发送到自行车仪表板的其余部分。这很有效，教室里的测量显示[布莱恩]以每小时 33 英里的速度踩踏板时产生了大约 450 瓦的能量。

下面视频。

[https://www.youtube.com/embed/Szhk8uvG0mk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Szhk8uvG0mk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)