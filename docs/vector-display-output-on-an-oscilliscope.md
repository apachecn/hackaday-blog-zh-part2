# 示波器上的矢量显示输出

> 原文：<https://hackaday.com/2014/02/19/vector-display-output-on-an-oscilliscope/>

![V3zirb1](img/a67f69f0a436e719e4439c7e10d883b2.png)

我们能说什么，我们是以我们的标志为特色的项目的吸盘。也就是说，这个真的很棒。[CNLohr]已经发现如何从 VGA 端口在示波器上创建矢量显示输出。

他的灵感来自于一款叫做[轨迹向量](http://www.youtube.com/watch?v=N1Dlhg6bea8)的游戏，这款游戏的玩法和小行星之类的一些老经典的玩法是一样的。这引起了[查尔斯]的思考，他决定看看如何制作他自己的矢量显示器。示波器非常适合这一点，因为它已经通过控制光束的位置(像矢量一样)来工作，而不是使用光栅化(水平扫描)的标准 LCD 和 CRT。这意味着，要让示波器显示图形，你需要做的只是改变进入 X 和 Y 通道的电压——嗯，速度要快！

但是你到哪里去找这样一个高速数模转换器呢？哦对了，你电脑的 VGA 端口！为了几美元,[Charles]用红色和蓝色输出([源代码](https://cnlohr.net/pubsvn/electrical/vga_multi/))拼凑了一个带有几个电阻的 VGA 适配器。一点编程之后，他创造了自己的矢量显示！

留下来看看我们可爱的头骨和十字扳手在他的示波器上旋转！哦，为了更深入的解释和更令人印象深刻的矢量视频演示。

[https://www.youtube.com/embed/vw1-E3Dxodc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vw1-E3Dxodc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/EfBwz_SiK8s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EfBwz_SiK8s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)