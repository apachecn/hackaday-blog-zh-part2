# 微型线路跟随器

> 原文：<https://hackaday.com/2014/01/15/miniscule-line-follower/>

![miniscule-line-follower](img/2744518539783283f35a46b226582428.png)

制造循线机器人既有趣又容易。建造这么小的线路跟随器是一个不同的故事。令我们惊讶的是，尽管它看起来很像，这个名叫 Rizeh 的机器人并不使用轮子来四处走动。[Naghi Sotoudeh] [使用两个振动马达](http://www.roborizeh.ir/)建造了线跟随器，针(上面未显示)与地面形成三点接触。

他的网站有点稀疏，但点击下载页面获得一个 PDF 文件，作为构建日志。我们还下载了 32 秒的演示视频，这是值得的。机器人环绕的魔标轨迹并不比你的手掌大多少！

在 diy PCB 上，您会发现两个 GP2S04 红外反射传感器，可以检测白纸上的黑线。上电序列需要几秒钟来校准这些传感器。说到电源，[纳吉]配备了蓝牙耳机的锂聚合物电池。其核心是 ATtiny45，它利用硬件 PWM 功能来驱动两个电机。

当然，排队等候者和[自动平衡器](http://hackaday.com/2012/07/20/self-balancing-robot-uses-cascading-pid-algorithms/)一起被列为我们最喜欢的机器人项目。但是到目前为止，我们最喜欢的是快速迷宫解决者[。](http://hackaday.com/2011/12/02/micromouse-wins-2011-maze-race-in-under-4-seconds/)