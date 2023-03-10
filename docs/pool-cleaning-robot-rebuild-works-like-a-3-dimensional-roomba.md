# 泳池清洁机器人重建工程就像一个三维 Roomba

> 原文：<https://hackaday.com/2014/08/17/pool-cleaning-robot-rebuild-works-like-a-3-dimensional-roomba/>

![Pool Cleaning Robot](img/c420e2a5c3c9928b02e8893933671d8c.png)

泳池很棒——清洗它们，不要太多。[大卫·吉罗尼]有一个泳池清洁机器人，但在氯环境中工作多年导致其中一个垫圈失效，破坏了里面的电子设备。他没有更换它，而是决定尝试用 AVR ATmega8 微控制器重建它。

但是等等！不是有保修吗？过期了。他不能从制造商那里拿块新的吗？几乎和新机器人一样贵——是时候打开它了！

他把这个项目分成两部分，出水计时器电路和机器人本身。计时器负责将 220VAC 转换为机器人的低压 DC，并根据时间表打开和关闭它(duh)。他正在使用一个基于 ATmega8 的倒计时可编程定时器，这是他为之前的项目设计的。

另一方面，机器人甚至更简单。它有两个马达，一个用来吸水过滤(也产生吸力效应，这样机器人就可以爬上池壁)，另一个用来操纵它。大卫在这里所要做的就是更换马达驱动器！

[https://www.youtube.com/embed/L1afAA2xByk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/L1afAA2xByk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)