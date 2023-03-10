# 从头开始制作薄膜键盘

> 原文：<https://hackaday.com/2015/01/25/making-membrane-keypads-from-scratch/>

几年前，[保罗]的儿子得到了一个简单的电子玩具，它能发出有趣的声音并给他唱歌。儿子喜欢这个玩具，但是在使用了一个又一个月之后，这个玩具不可避免地坏掉了，无法修复。设想一个“播放声音的电子盒子”并不是一个很难复制的项目，[保罗]开始着手制作他自己的。电子设备并不难，但定制的薄膜键盘很难获得。没关系，[因为构建自己的](http://paulbleisch.com/blog/2015/01/19/custom-arduino-membrane-keypad/)其实很容易。

薄膜开关通常是用丝网印刷的导电油墨在花式塑料上制成的，但这并不是制作自己的薄膜开关的必要条件。你真正需要的是四层——一个“正面贴花”,一个用于行的“顶部箔”层，一个用于列的“底部箔”层，以及一个在行和列之间提供足够间隔的“剪切”层。

[Peter]在 Illustrator 中布置四个图层，打印图层，并用铜带覆盖行和列。剪切层是保持各层分离的关键部分，直到按钮被按下，这只是一张带有精心放置的孔的卡片。

一旦行、列和其他层被粘合起来，[Peter]就可以将这个键盘连接到微控制器上。Arduino 键盘库的代码非常简单，应该经得起孩子操作的考验。