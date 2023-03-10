# DIY 刺绣机把你的名字缝在你的内衣上

> 原文：<https://hackaday.com/2014/06/10/diy-embroidery-machine-sews-your-name-in-your-undies/>

![DIY Embroidery Machine](img/f3d217c73a3eb920de36f82d306f7add.png)

如果你想在市场上买一台有刺绣功能的缝纫机，你要么花一大笔钱，要么满足于一台成本较低、只能完成少量预编程设计的机器。一个名叫[SausagePaws]的 DIYer 想出了第三个选择，他会自己做一个。他也很有动力，SausagePaws 夫人]想要一个！

一个现成的刺绣机类似于一个标准的缝纫机，除了面料的运动是自动完成的，而不是用手。工件不仅在移动，而且必须随着指针的上下移动而及时移动。[SausagePaws]采取了一种严肃的方法，并决定最简单的方法是在 XY 驱动系统的末端安装一个[刺绣环](http://en.wikipedia.org/wiki/Embroidery_hoop)。

![DIY Embroidery Machine](img/951d072d9c569b2ac131eeed566aa377.png)

X 和 Y 轴由 NEMA 17 步进电机、同步带和骑在铝挤压上的 v 形轮组成。关于针位置检测是如何完成的，没有很多可用的信息。然而，有提到使用弹簧钢…也许当指针向上移动时，它接触弹簧钢，闭合电路，有效地成为开关。

自定义编写的应用程序与 PIC 微控制器通信，PIC 微控制器根据设计文件和针位置提供步进电机控制。不幸的是，没有提供关于 PIC 代码或控制器应用程序的信息。即便如此，这也是一个不错的项目，并表明它是可以完成的。

[https://www.youtube.com/embed/u6JFxtSsWpw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u6JFxtSsWpw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)