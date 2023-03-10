# 将立体声添加到单声道音频

> 原文：<https://hackaday.com/2013/05/22/adding-stereo-to-monophonic-audio/>

![board](img/402e1cbbc5d230438159620de10103d4.png)

上个学期，康奈尔大学的布鲁斯·兰德实验室里发生了许多令人惊叹的事情。三名学生——[Pat]、[Ed]和[Hanna]投入了数小时的工作来开发一些算法，这些算法能够用单声道声音模拟立体声音频。这足够完成[兰德博士]的 ECE 5030 课程三个学期的工作，虽然不可能通过 YouTube 视频真正欣赏这个项目，但我们假设这是一件了不起的作品。

该团队项目的第一部分是收集关于人耳在 3D 空间中听觉的数据。为了做到这一点，他们在一名队员的耳朵上安装了麦克风，让他们坐在一个旋转的凳子上，然后播放一系列的咔嗒声。大量的 MATLAB 之后，这个团队有了一个他们的团队成员的头部如何听到声音的平均值。基本上，他们创造了一个双声道录音如何工作的算法。

为了证明他们的算法是可行的，该团队将一段音乐压缩成单声道，并通过 MSP430 微控制器播放。有了一副好的耳机，他们能够将音乐虚拟地放入立体声空间。

下面的视频涵盖了他们的基本建设，但由于[布鲁斯]的相机和 YouTube 的限制，你将无法亲自体验该团队的虚拟立体声。然而，你可以戴上一副耳机[来听这个](http://www.youtube.com/watch?v=IUDTlvagjJA)，这是一个很好的例子，说明了这种设置可以做什么。

[https://www.youtube.com/embed/tzuu5gRPN50?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tzuu5gRPN50?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)