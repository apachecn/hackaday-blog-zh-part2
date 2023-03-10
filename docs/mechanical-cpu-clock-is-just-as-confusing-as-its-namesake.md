# 机械 CPU 时钟就像它的名字一样令人困惑

> 原文：<https://hackaday.com/2012/04/16/mechanical-cpu-clock-is-just-as-confusing-as-its-namesake/>

![](img/4353e9ce005075ee995a91d06b52b568.png "mechanical-cpu-clock")

[Lior Elazary]设计并[制造了这个时钟来模拟 CPU](http://www.liorelazary.com/index.php?option=com_content&view=article&id=46:mechanical-cpu-clock&catid=10:clocks&Itemid=15) 的功能。问题是，如果你还没有很好地掌握一个 CPU 是如何工作的，我们认为这个时钟将会令人困惑。但幸运的是，我们得到了它，我们爱它！

小时数据在寄存器 a 中显示为二进制数，这是红色部分的中间一列，MSB 在底部，LSB 在顶部，左指位的功能为数字 1。时钟缺乏显示任何其他时间数据所需的复杂性。不过没关系，因为滚珠轴承每分钟落下时发出的声音可能会让你有点抓狂。[Lior]没有谈到运送滚珠轴承的机制，但你可以从休息后的视频中看到，一个圆形路径上的磁铁将它捡起来，并将其运送到时钟的顶部，在那里重力用于给寄存器供电。有两条轨道可以让球绕过 A 寄存器，向右进入 B 寄存器。当计数大于 11 时，它与寄存器 C(在左侧)一起复位小时数。

如果你需要了解这些机械加法器是如何组装在一起的，看看这个木制加法器项目。

[https://www.youtube.com/embed/0H4LTOYpAM4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0H4LTOYpAM4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)