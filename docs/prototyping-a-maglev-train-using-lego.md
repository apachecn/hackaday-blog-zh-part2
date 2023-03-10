# 用乐高制作磁悬浮列车的原型

> 原文：<https://hackaday.com/2013/06/26/prototyping-a-maglev-train-using-lego/>

![lego-maglev](img/9d1c1a56b34ef46a9700c2f364bb1d5a.png)

使用不那么严肃的设备进行严肃的研究？我们对此一无所知。[用乐高做磁悬浮](http://www.theonerobot.com/maglevresearch)的研究平台有什么问题？这个团队已经这样做了一段时间，并取得了很大的成果。

磁悬浮列车是一种基于磁悬浮原理的交通工具。相似磁极的磁铁互相排斥，这一概念可用于创建一个无摩擦的轨道系统。但是这也带来了刹车和移动的问题。上面链接的构建日志涵盖了研究项目第八次迭代中的概念。但是下面的视频对他们解决这些问题的方法提供了最简洁的解释。

研究人员使用放置在轨道沟槽中的磁铁作为一种磁性装置来推动。乐高车上的一系列电磁铁在轨道上运行。可以通电，作为线性电机推动这些永磁体。但是你怎么知道这会导致哪个方向的旅行呢？这个问题通过在每个电磁铁之间增加一个霍尔效应传感器得到了解决。在接通线圈之前，霍尔效应传感器被轮询，并且基于它们的值选择定时方案。这是用来推动列车加速，以及减速制动。

[https://www.youtube.com/embed/7xX5nZ_MUGs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7xX5nZ_MUGs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/arduino/comments/1gjc8k/arduinocontrolled_lego_maglev_vehicle/)