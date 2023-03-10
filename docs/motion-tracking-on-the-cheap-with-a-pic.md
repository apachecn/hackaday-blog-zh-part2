# 使用 PIC 实现廉价的运动跟踪

> 原文：<https://hackaday.com/2014/02/13/motion-tracking-on-the-cheap-with-a-pic/>

![motion tracking](img/d751f1e6dbab531fe4c743904919fc4e.png)

曾经需要一个便宜的运动跟踪器来跟踪最基本的物体吗？你知道吗，你可以用几个红外距离传感器和一张照片组合成一个。

设置相当简单。[Aron Horan]正在使用 dsPIC30F4011 PIC、夏普红外距离传感器、RC 伺服和 PICkit2 进行测试。它通过使用伺服电机左右扫描来工作。当检测到对象的边缘时，它将远离该对象，直到它不再能够检测到边缘，然后它返回。不幸的是，这意味着它会一直抽搐，即使是在追踪一个物体的时候。

像[Aron]记录的许多其他项目一样，他包括了你需要知道的一切，以便能够自己重新创建这个项目。流程图、接线图和代码——当然是用 C 语言写的！下面的视频包括一个出色的演示，但如果你想直接跳到行动，你可以看到它在大约 0:39 in 开始跟踪一个万用表。

[https://www.youtube.com/embed/7MUBVgCZxYk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7MUBVgCZxYk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

红外传感器眼熟吗？这是因为我们最近推出了[Aron]的另一个项目，Dodgebot！