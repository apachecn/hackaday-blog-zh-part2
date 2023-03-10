# 机器人打游戏机大战

> 原文：<https://hackaday.com/2015/03/28/in-which-robots-fight-the-console-wars/>

虽然这些年来名字已经变了，但游戏机大战仍在继续。[moop]在开始他目前的项目 [Foobot](http://www.moop.org.uk/index.php/2015/03/15/foobot/) 时，一定很怀念 NES 对 SEGA 的日子，这是一款桌面足球游戏，由机器人玩，用经典的 NES 和 SEGA 控制器控制。

每个小组都有两个机器人，在直接连接到 16,000RPM 马达的激光切割有机玻璃轮子上工作。一个 SN754410 控制电机，每个机器人都有一个 ATtiny2313 大脑。它们都通过各自的 433MHz 1402 无线电接收器模块与单个发射器进行通信。为了避免冲突，[moop]使用了一种分组系统，其中每个机器人都有一个 id。这些消息都包含机器人 ID、消息有效载荷和校验和。机器人忽略发给其他人的消息，以及任何带有无效校验和的消息。

[moop]在他的 [github](https://github.com/mooped/foobot) 上提供了一切，包括机器人底盘和发射器外壳的 PCB 布局和 CAD 文件。休息之后看他们决一胜负。如果这些机器人让你对老式游戏感到愤怒，看看[这些可爱的街机黑客](http://hackaday.com/2014/09/12/hacklet-15-arcade-fire/)。

[https://www.youtube.com/embed/WSiUapAQzWc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WSiUapAQzWc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [危险原型](http://dangerousprototypes.com/2015/03/17/foobot-a-robot-table-football-game/)