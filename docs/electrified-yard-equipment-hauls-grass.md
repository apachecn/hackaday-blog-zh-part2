# 电气化庭院设备拉草

> 原文：<https://hackaday.com/2013/10/02/electrified-yard-equipment-hauls-grass/>

![mower2](img/9e118f6037690ad13568caee276df0c5.png)

[AmpEater]花了一个夏天[将庭院设备从内燃转换成电力](http://upstateelectric607.wordpress.com/)。转换运行从一个相对驯服的车轮马，到一个疯狂的幼兽学员。车轮马失去了它的科勒发动机，取而代之的是皇冠叉车的液压泵马达。48 伏电源由 MK 铅酸凝胶电池提供。一个 Alltrax 300 安培控制器控制着这匹马。

[在他的 Reddit 帖子上](http://www.reddit.com/r/electronics/comments/1ncktk/zero_emission_lawn_mower_conversions_and/),[ AmpEater]说他特别为他的新手学员 zero turn 乘割草机感到骄傲。对于那些不熟悉草坪工具术语的人来说，“零转弯”意味着割草机的转弯半径为零。零度转向割草机使用两个大轮子和坦克式转向，在自己的半径范围内转弯。我们打赌这种类型的割草机也将成为一个很好的[机器人转换](http://hackaday.com/2011/08/25/how-not-to-build-a-robotic-lawnmower/)，但是【安培特】的零转弯仍然是为了割草而设置的。

在拉动 V 型双马达后，48 伏 Motenergy ME-1004 被放置到位。电池是 3 个 Enerdel 48V 33 安培小时的锂离子电池组。电池组串联连接，提供 144V 标称电压。就在这里，我们的大脑开始融化。144 伏上的 48 伏电机意味着魔法烟雾，对吗？这就是电机控制器神奇的地方。

【AmpEater】使用 Evnetics 孤子-jr 电机控制器。该控制器似乎是作为一个直流到 DC 转换器运行，将电机的 144v 降至安全的 48v，并提供了许多其他功能。即使使用开关降低电压，控制器中也会产生大量热量。孤子具有液体冷却能力，并且[AmpEater]正在试验一种库蕾丝 PMP-450 系统。我们有点担心一个电脑冷却系统经得起振动和滥用 50“割草机可以菜了。

如果你想知道，这不是一个便宜的转换。马达的零售价超过 500 美元，控制器约 2100 美元，电池每包约 4500 美元。这比初级学员的原价高出一倍多。可以理解的是，这些转换超出了普通房主的能力范围，但是对于商业园丁来说却是值得的。即使最近推动四冲程发动机，小型发动机仍然是主要的污染源。我们希望我们可以说电动割草机比燃气割草机更安静，但是正如视频所示，割草机产生的大部分噪音是刀片本身产生的。

[https://www.youtube.com/embed/V7SatHgu5jk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/V7SatHgu5jk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)