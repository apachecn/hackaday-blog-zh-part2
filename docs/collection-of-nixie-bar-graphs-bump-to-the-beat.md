# 谢妮棒图合集

> 原文：<https://hackaday.com/2012/11/05/collection-of-nixie-bar-graphs-bump-to-the-beat/>

![](img/3e500e56c5bd5fa14d376f8a34e44d0e.png "bar-graph-nixie-bumps-to-the-beat")

这个 [VU 计使用谢妮管作为显示器](http://tchips.com/nixie-music-visualizer)。总共有 14 个 13 英寸条形图管来绘制音频频谱。构建纯粹使用硬件来显示；没有使用微控制器处理或专用的 VU 计芯片。

输入始于一个双通道运算放大器和一对电位计，可以平衡左右声道。然后，两个通道都被分成七个信号，这解释了上面看到的电子管布局。然后，每个信号通过一个分压器，将输出包络在 0V 至 6V 之间。还有一个低通滤波器来处理突然的音量峰值，这对于 nixies 来说不是很好。但正如休息后的视频所示，所有的工作都得到了回报。这个片段让我们看到了绿色的原板，它承载了所有这些过滤硬件。在使用扫频来测试系统的前两个演示中，您可能会想调低音量。

[https://www.youtube.com/embed/qLzXueWH8qo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qLzXueWH8qo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)