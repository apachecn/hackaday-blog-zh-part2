# PicoRico Hacks 自行车悬挂遥测字符串编码器

> 原文：<https://hackaday.com/2015/05/12/picorico-hacks-string-encoder-for-bike-suspension-telemetry/>

它很简单，很优雅，而且效果非常好。PicoRico 团队为下坡自行车建造了[遥测系统。想一想，你会怎么做？嗯，遥测很容易…只需添加一个 IMU 板，你就万事大吉了。他们不仅如此，还计划走得更远。事实上，惯性测量组合是后来才想到的。这个建筑的精华是一个传感器，它可以有几个名字:弦编码器，拉线传感器，弦点，等等。但是有两件事是肯定的，他们为他们的黑客马拉松构建做了很好的计划，并且执行了这个计划。这使他们在 2015 年纽约 Disrupt Hackathon 上获得了最高奖项](https://hackaday.io/project/5606-picorico)的亚军[，并在该活动中获得了最高黑客日奖。](http://techcrunch.com/2015/05/03/disrupt-ny-2015-hackathon-winners/)

![picorico-thumb](img/4e68c823e7bb579b38b3d9c6a2c6bda5.png)、[Marek]和[Dorian]想要记录[Chris]下坡自行车的所有遥测数据。最大的挑战之一是测量前叉上悬架吸收的力。这三个人之前已经尝试过几次了。他们使用一种可伸缩的电线，就像保管人腰带上的钥匙一样，配合一个电位计来测量变化。这就是 stringpot 这个术语的由来。问题是你的分辨率和灵敏度不是很可靠。

这是传感器的问题，而不是机械问题，所以他们保留了可伸缩的卷轴，并用一个更可靠的部件替换了罐子。取而代之的是 AMT203 绝对位置传感器，提供了史诗级的检测。根据[数据手册](http://www.cui.com/product/resource/amt20-v.pdf) (PDF)该 SPI 器件检测 12 位旋转数据，可以通过 SPI 总线调零，精度达到 0.2 度。不幸的是，我们没有得到一个很好的安装特写镜头，但它显示在视频中。编码器和卷收器安装在减震器上方，线向下延伸到扦状物。当震动启动时，绳子伸缩，转动绝对编码器。将此与 IMU(以及他们计划添加的另外两个 IMU)结合起来，您就有了大量数据来绘制和分析。休息后的视频展示了字符串编码器的演示和对团队的采访。

## 他们来玩了

值得注意的是，PicoRico 团队赢得了这场比赛。他们为 20 小时的黑客马拉松赛(T1)打包了大量行李。这里有一张他们参加活动时所带的所有装备的照片…除了自行车本身。

我们看到了焊接站、Dremel(带钻床)、冲击式驱动器、丝锥和模具、延长线、装满电子产品的箱子等等。这种类型的规划打破了硬件黑客马拉松经常面临的障碍。可以下载一个软件库；你不能下载任何人都没有的工具或建筑材料。这也是我们从[Kenji Larsen]那里学到的经验，作为他在活动中指导的一部分，他带来了一个装在滚筒袋中的移动制造设备。

如果你开始进入黑客马拉松，我们希望你会，请记住这一点。在活动开始前尽可能多地集思广益，带上你信任的装备一起去。

[https://www.youtube.com/embed/vzF9AYtiXwo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vzF9AYtiXwo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Oji3_4bvjaU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Oji3_4bvjaU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)