# 我的机器人军队@创客节

> 原文：<https://hackaday.com/2015/06/02/my-robot-army-maker-faire/>

几年来，我一直在开发一个交互式三角洲机器人部队。这个正在进行的项目是由我控制许多机械四肢的愿望推动的，就像我身体的延伸一样(我假设我不是这里唯一一个幻想机器人的人)。

由于我的军队没有实际应用……除了产生漂亮的光图案，让用户在一分钟内感觉非常酷，我猜你会称之为艺术。过去，我举办了一个 [Kickstarter](https://www.kickstarter.com/projects/1984252088/robot-army-starter-kit) 来资助我的艺术创作，现在我可以愉快地在有趣的活动中展示这些作品；创造者大会就是其中之一。

## 交互性和庞大的人群

去年，[在大湾区创客节](http://hackaday.com/2014/05/30/robot-army-irl-plus-a-massive-build-log/)上我们首次亮相，我和我的合作者【Mark】展示了一个较小的 30 个机器人样本，用于我们的安装。我们还决定创建一个交互式的方面供其他人体验。在去年 3 月我们的众筹期结束后，我们有一个多月的时间在大型活动之前做任何开发，所以我们的选择很少。简单的解决方案是将我们的 delta 代码插入 Xbox Kinect 的[Open NI](https://code.google.com/p/simple-openni/)with[Processing](https://processing.org)的手部追踪演示中。这很酷，足以展示，但我们真的没有预料到它会在像 Maker Faire 的暗室这样拥挤的环境中如何发展。

我们应该早就知道了。我们两个都意识到会有很多很多的孩子…都用微型的手来迷惑 Kinect，但是我们还是做了。我们唯一的决心是实现一个功能，迫使 Kinect 一次跟踪一只手，*只是在以一种非常特殊的方式挥手之后*。在需要向每个周末路过我们展位的人解释这一规定后，我们决定再也不在人群中使用 Kinect 吸取教训。

## 三角洲机器人和 DMX

在过去的一年里，自从那次经历之后，我们已经将安装的规模扩大了两倍，并且想出了一些更好的演示想法。到目前为止，机器人都可以通过 RS485 总线单独寻址，我们通过 CAT5 电缆使用 DMX 协议发送命令。如果你不熟悉它，DMX 在演出制作中被用来控制舞台灯光……对此有一个超级简洁和免费的应用程序叫做 [QLC+](http://www.qlcplus.org) ，它可以让你有效地编排许多单个灯光单元的运动和颜色；非常适合我们的事业。

在功能上，装置中的 84 个 delta 机器人中的每一个都认为自己是舞台灯(有身份问题的机器人)。我们将末端效应器的 X 和 Y 轴映射到现有的平移和倾斜值，并将 z 轴映射到光束聚焦值。安装在每个 delta 的末端效应器中的 LED 的 RGB 直接映射到舞台灯光的 RGB 值。

通过使用 QLC+ GUI 中的滑块，我可以选择机器人组，并为位置和颜色创建预置。这太棒了，像我这样不怎么写代码的人可以不费吹灰之力就编出令人印象深刻的舞蹈。此外，该程序附带了一个很好的可视化工具，您可以在其中布局虚拟节点，并在开发它们时查看您的效果。

这是我们在 QLC+绘制的安装布局图。每个灯周围的蓝绿色和紫色滑块代表平移和倾斜(在我们的例子中是 X 和 Y):

![QLCdelta](img/6428a837fe9e83f0d8ab5dadc376879e.png)

照明控制是一个有趣的解决方案。今年拥有自主机器人改变了人们对它们的反应，因为它们不像是你指挥的军队，而更像是一片发光的草地。

[Mark]我和我正在考虑挑选一些 flex 传感器，也许可以玩玩 Leap 或 EEG 耳机，作为重新引入互动方面的一种方式。总之，我有一个很酷的新玩具，我迫不及待地想玩一个夏天！

[https://www.youtube.com/embed/YkIscsf_pUc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YkIscsf_pUc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/AwHTOyvZh3c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AwHTOyvZh3c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)