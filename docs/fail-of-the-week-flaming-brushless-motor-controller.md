# 本周失败:燃烧的无刷电机控制器

> 原文：<https://hackaday.com/2013/10/24/fail-of-the-week-flaming-brushless-motor-controller/>

是的，烟雾和火焰通常是你的电子设备没有按预期运行的迹象。这其实是[在学习无刷电机控制器](http://www.mikekohn.net/micro/brushless_motor.php)时遇到的第二个故障。

[Michael Kohn]在为另一个项目工作时购买了马达，它闲置了很长一段时间。当他再次遇到它时，他决定他应该学习 BLDC 控制的不那么黑暗的艺术。

第一个障碍是弄清楚如何驱动三线电机，而他原本预计只有两个。答案要求他想出一种开关机制，允许每根电线有三种状态:正极、负极和未连接。他的解决方案是使用 MOSFETs。这是一个好主意，但不幸的是，在第一次迭代中，它们的规格不足，当其中一个在测试中爆炸时，他吓坏了。在采购了一套更坚固的金属氧化物半导体场效应晶体管后,[迈克尔]回去进行测试，这时这场小火灾就爆发了。连接锂电池和驱动器的 22 号电线无法切断它。在第二个片段中，你可以看到。

从我们说这句话到现在已经有一段时间了:请记住，本周的失败不是嘲笑那些慷慨地记录了自己失败的黑客。这是关于从错误中学习，并讨论未来可以帮助他人的替代方案。例如，在这种情况下，为任何类型的电机确定 MOSFET 规格和线规的一些建议将非常有帮助。请在评论中关注它。

[https://www.youtube.com/embed/3VyduGaUq1g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3VyduGaUq1g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/FPuvoUMzCW0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FPuvoUMzCW0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**