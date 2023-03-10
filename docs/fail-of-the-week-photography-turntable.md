# 本周失败:摄影转盘

> 原文：<https://hackaday.com/2013/10/10/fail-of-the-week-photography-turntable/>

在网上购物的推动下，转盘摄影越来越受欢迎。如果你不能把它拿在手里，至少你可以从各个角度看到它的样子。从静态图像来看，【Petteri Aimonen 的】[自卷转盘看起来很棒](http://essentialscrap.com/spinplate/)。它是完全封闭的，并且油漆得非常好。但是当你看到它的动作时，它似乎有点口吃。

[https://www.youtube.com/embed/uHyJL9CM6K0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uHyJL9CM6K0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

他不只是用这个来捕捉连续旋转的视频，而是计划让它旋转一个设定的量，然后在拍摄图像时暂停。他用一个 STM32 微控制器来驱动一个无刷电机，这个无刷电机是他从一个硬盘中取出来的。它完全可以工作，但是硬盘马达的性质阻碍了他最初的计划。它意味着以非常高的速度低摩擦地运行。但是这东西从来就不是设计来一毛钱就停下来的。所以当它被定向转三十度的时候，就超调了，像视频里那样来回振荡。

这种振荡会持续十几秒钟。但是[佩特里]能够通过在圆盘上增加一些摩擦力来抑制它。他还必须调整原始驱动器设计，添加他忘记包含的反激二极管，并处理向线圈馈送 PWM 信号时引起的一些问题。还有其他一些小的失败也在折磨着他。油漆颜色与他使用的灯箱不匹配，电池有一些问题，有一次他从 PCB 上折断了编程头。尽管有这些令人沮丧的问题，我们仍然打赌在这个项目上工作是非常有趣的。

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**