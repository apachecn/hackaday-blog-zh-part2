# Hyperlapse 让你的摄像头视频棒极了

> 原文：<https://hackaday.com/2014/08/12/hyperlapse/>

第一人称视频——在谷歌眼镜、GoPro 和其他运动相机之间，似乎每个人的头上都有一台相机。如果你是冲浪者或跳伞运动员，那可能会拍出一些精彩的镜头。但对我们其他人来说，这意味着数小时无聊的视频。解决这个问题最明显的方法是延时拍摄。通常情况下，延时会丢弃帧。每 10 帧取 1 帧，速度提高 10 倍。不幸的是，加快头戴式相机的速度往往会导致视频非常有弹性，没有晕机袋就无法观看。微软研究院的约翰尼斯·科普夫、[迈克尔·科恩]和[理查德·塞利斯基]想出了一个解决这个问题的新方法，用[超光速](http://research.microsoft.com/en-us/um/redmond/projects/hyperlapse/)。

[超延时摄影](http://en.wikipedia.org/wiki/Hyperlapse)不是一个新名词。通常情况下，超延时电影需要仔细的规划、摄影机装备和劳动密集型的后期制作，才能获得可用的视频。[Johannes]和他的团队已经将计算机视觉和图形算法投入到这个问题中。结果简直令人吃惊。

完整的细节可在[团队报告](http://research.microsoft.com/en-us/um/redmond/projects/hyperlapse/paper/hyperlapse.pdf)中获得(35MB PDF 警告)。为了获得有用的数据，必须校准这些相机上常用的鱼眼镜头。这个团队用 [OCamCalib 工具箱](https://sites.google.com/site/scarabotix/ocamcalib-toolbox)完成了这项工作。导入的视频被逐帧分解。使用来自运动的[结构](http://en.wikipedia.org/wiki/Structure_from_motion)算法，hyperlapse 创建了视频中各种场景的 3D 模型。有了这个虚拟世界中的场景，相机可以随意移动和瞄准。该团队的算法然后选择一条平滑的路径，沿着原始相机轨迹。一旦知道了摄像机的位置，渲染最终的视频就简单了。

结果并不完美。爬山场景显示了由相机帧速率和曝光因变化的照明条件而改变所引起的一些伪像。人们在视频的骑自行车部分出现和消失。

团队没有提到的一件事是这个过程需要多长时间。我们确信这种渲染一定需要大量的时间和处理能力。尽管如此，输出视频是惊人的。

概述视频

[https://www.youtube.com/embed/SOpwHaQnRSY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SOpwHaQnRSY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

技术细节

[https://www.youtube.com/embed/sA4Za3Hv6ng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sA4Za3Hv6ng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢[古斯塔夫]！