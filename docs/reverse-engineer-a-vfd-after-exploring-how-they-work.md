# 探索 VFD 的工作原理后，对其进行逆向工程

> 原文：<https://hackaday.com/2015/03/04/reverse-engineer-a-vfd-after-exploring-how-they-work/>

[达夫·琼斯]得到了一个真正的宽，两行真空荧光显示器。我们以前在旧设备中遇到过这些装置，你可以从通常的来源得到它们，不管是新的还是旧的，但是你需要知道如何驾驶它们。最近一期的 [EEVblog 逆向工程这个 VFD](https://www.youtube.com/watch?v=clUVEyi_YNM) 。

这些显示器的功能非常容易理解，在休息后的视频中[Dave]会介绍这一点。有阴极线和磷光涂层阳极。当施加电流时，阳极发光。为了增加对哪些阳极发光的控制，在阳极和阴极线之间放置一个网格。对栅极施加负电位会阻止电子向阳极移动，因此该区域不会被点亮。

现在驱动这种低级的东西并不容易，但请放心，你找到的大多数 VFD 都将有一个驱动程序连接到它们。逆向工程就是找出用来控制驱动程序的协议。该板上有一个 2 引脚连接器，带有一个大的电解滤波电容，是电源轨的绝对赠品。看着直接连接的板载处理器，他确定输入将被 5V 调节，因为这是芯片所期望的。连接他的工作台电源会产生一个闪烁的光标！[Dave]继续抽取并行数据并使用 Arduino 测试控制引脚。他找到了成功，一路上分享了许多伟大的逆向工程技巧。

我们经常称这种类型的东西为黑暗艺术，但那真的只是因为没有多少人愿意尝试一下。我们认为这需要改变，所以遵循这个例子，也去看看[Ben hecken dorn]最近的[LCD 逆向工程](http://hackaday.com/2015/01/29/reverse-engineer-then-drive-lcd-with-fpga/)，然后拿一些设备，给自己一个尝试。[我们想听听](http://hackaday.com/submit-a-tip/)你的成就！

[https://www.youtube.com/embed/clUVEyi_YNM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/clUVEyi_YNM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[Thanks Indrora]