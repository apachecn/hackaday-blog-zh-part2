# hacklet 36–示波器项目

> 原文：<https://hackaday.com/2015/02/27/hacklet-36-oscilloscope-projects/>

示波器是工程师、黑客或制造商最常用的工具之一。电压表可以做很多事情，但当你真的需要好好观察信号时，一个好的示波器是非常宝贵的。本周的黑客攻击是由 [Hackaday.io 上一些最好的示波器项目的上升斜率引发的！](http://hackaday.io/)

[![rigol500](img/3991cc8fc1bfc20c6e6c98238a9fec79.png)](http://hackaday.io/project/4327) 我们从【DainBramage】最近的项目[开始，延伸一个 Rigol DS-1102E 示波器的极限](http://hackaday.io/project/4327)。新的 Rigol ds1054z 最近可能会受到所有媒体的关注，但旧的 DS-1102E (100 MHz)型号仍然是一个非常有能力的示波器。[DainBramage]拿出他的 vintage Singer CSM-1 服务监视器，产生高达 500 MHz 的频率。Rigol 的表现令人钦佩，可以检测到高达 500 MHz 的正弦波。这部分是由于示波器每秒 1 千兆采样的采样率。然而，一旦超过 100 MHz 的特定限制，信号就开始衰减。不坏的推动低端范围超越其限制！

[![cornel-scope](img/e91db56c24bb0fce82764bee5fcde02f.png)](http://hackaday.io/project/2032) 接下来是【布鲁斯·兰德】带着他的 [PIC32 示波器](http://hackaday.io/project/2032)。微控制器范围项目并不新鲜，但一个以近 1 MHz 的采样速率运行，同时生成 NTSC 复合视频的项目是不容忽视的。[Bruce]通过使用直接内存访问(DMA)将数据从 ADC 移至内存，并将视频数据从内存移至用于生成视频的 I/O 引脚，实现了这一点。视频本身是由电阻树 DAC 创建的。制作黑白视频只需要三个电阻和两个 I/O 引脚。[Bruce]说整个范围的零件价值约 4.00 美元！

[![scope-hand](img/3dbcc5793282bd852a8aa078e9f2d802.png)](http://hackaday.io/project/3239) 【雅各布·基督】用他的 [chipKIT 示波器绘图仪](http://hackaday.io/project/3239)混合了艺术和科学。[Jacob]使用基于 Fubarino 的微芯片 PIC32 在他的瞄准镜上绘制图案。为此，必须将示波器设置为 X-Y 模式。[Jacob]将他的 Fubarino 与 MCP4902 数模转换器(DAC)配对。使用专用 DAC 是一种很好的方法。[Jacob 的]图像就是一个证明，因为它们是我们见过的最干净的“范围艺术”绘画。很像[布鲁斯·兰德]，[雅各布]用他的项目作为大学课程的基础。事实上，左边的图片是他的一个学生创作的！

想要更多范围的好处吗？查看我们新的[示波器项目列表！](http://hackaday.io/list/4460-oscilloscope-projects)

#### Hackaday.io 更新！

[Hackaday.io](https://hackaday.io) 每天都在获得新功能。我们的开发团队刚刚推出了一个新的画廊视图。只需点击项目的特色图像或“查看图库”按钮，您将看到项目中使用的所有图像的图库视图，包括日志图像。YouTube 视频也将在图库中呈现。这是在 hackaday.io 上查看一些项目进展时间表的一个很好的方式。要查看这方面的一个很好的例子，请查看 [OpenMV 的图库](http://hackaday.io/project/1313/gallery)。

在其他 Hackaday.io 新闻中，请查看[标题 CERN 竞赛！](http://hackaday.io/contest/4200-caption-cern-contest/log/14467-caption-cern-contest-week-4)每周我们都会从 CERN 的档案中上传一张新的图片。想出最有趣标题的 Hackaday.io 用户将赢得一件来自[hack aday 商店的 t 恤！](http://store.hackaday.com/)

看起来我们已经追踪到这个黑客攻击的终点了。同样的黑时间，同样的黑渠道，带给你最好的 [Hackaday.io！](http://hackaday.io/)