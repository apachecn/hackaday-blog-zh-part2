# 奖励时钟很好地用作台秤

> 原文：<https://hackaday.com/2013/01/21/award-clock-put-to-good-use-as-a-bench-meter/>

![award-clock-turned-voltage-meter](img/3e77537ad949adeb42203f55d156e0fa.png)

激励行业生产了数百万的这种奖励饰品。这里有一个实际使用它的方法。时钟表盘不是显示时间，而是显示电压表的读数。

当我们第一次看到这个帖子时，我们认为黑客使用了某种类型的线圈注射来驱动指针。但事实证明这是机械驱动的。上图显示了安装在时钟后面的步进电机。它的驱动轴与时钟背面的调节旋钮相连。马达的精度使 PICAXE 能够根据马达的步数设置时钟表盘。时针以分钟为单位显示十位数值(基数为 10，而不是基数为 60)。这意味着最高可测量电压为 12V——当时针位于 12 时，测量值为 0 伏加上分针的十分之一伏。拨号盘搞定后，项目的其余部分将重点放在使用 ADC 测量电压上，ADC 的上限仅为 5V。这可以通过一个简单的分压器来解决。

休息后，你可以看到钻机的准确性，因为它旁边的数字电压表进行测量。

[https://www.youtube.com/embed/vQu-uB6nVNo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vQu-uB6nVNo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢帕特]