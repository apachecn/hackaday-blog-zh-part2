# 超级粉碎兄弟得到了微软 Kinect 改造

> 原文：<https://hackaday.com/2014/10/26/super-smash-bros-gets-a-revamp-with-the-microsoft-kinect/>

[Eric]刚刚发来了这个他和几个朋友一起做的很棒的 Kinect 黑客。用 Kinect 玩超级粉碎兄弟。

该系统使用了两台 Kinects 和三台电脑。第一个 Kinect 记录每个玩家的移动，而第二个 Kinect 则观察两个玩家互相“战斗”。第一台 PC 运行任天堂 64 模拟器来玩游戏。![character selection](img/e66ab1a38e53d4f266af08359056cc6e.png)

第二台 PC 运行带有 OpenCV 的摄像头，以添加另一个很酷但可能不必要的功能，你看，即使是角色选择也是一个物理过程，增加了用身体玩整个游戏的想法。玻璃桌子允许玩家将他们的 3D 打印令牌放在玻璃上，有效地将其放在他们想要使用的角色上。

当比赛结束时，一个挡风玻璃刮水器将输掉的玩家的代币从桌上打掉。

第三台电脑负责运行两台 Kinects，然后必须通过 TCP 连接将生成的命令发送回第一台电脑，以便输入到游戏中。

他们[在由戴尔和英特尔赞助的 2014 年秋季黑客大赛 MHacks 上向公众](https://www.youtube.com/watch?v=eUhwQlD0EJY&feature=youtu.be&t=1h57m10s)介绍了它。下面视频。

[https://www.youtube.com/embed/S6H04SD3SDI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/S6H04SD3SDI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们都看到了最近关于用 Kinect 玩超级马里奥兄弟的帖子，这就引出了一个问题，为什么没有更多的游戏被转换？嗯……除了用你的身体很难玩这个事实之外……