# 棋盘步序器

> 原文：<https://hackaday.com/2012/04/18/chess-board-step-sequencer/>

[tinkartank]来信告诉我们他制作的[棋盘步序器](http://tinkartank.wordpress.com/2012/04/17/the-chess-sequencer/)。这是一个伟大的作品，结合了美妙的古典知识，一套棋子赋予现代技术的音乐设备，如单体。

建造开始时，在每一个方块下面钻一些小孔，并安装非常小而脆弱的簧片开关。64 个这样的开关连接成行和列，然后连接到 Arduino Mega 的数字输入端。为了关闭这些簧片开关，磁铁被植入每个棋子的底部，这样每当棋盘上的一个棋子移动时，电路就会闭合。

在控制方面，[tinkartank]建立了一个非常好的控制面板来改变正在播放的键*、速度、琶音转盘、步数，以及音符之间是否有一个完整或半步。有了这个控制面板，[tinkartank]几乎可以演奏任何音阶。

听起来怎么样？嗯，Arduino Mega 输出的 MIDI 非常逼真，听起来像任何可以想象的东西。从视频演示(休息后可用)来看，我们真的很喜欢这个界面，一个簧片开关阵列棋盘正在慢慢爬上我们的“要构建”列表，如果仅仅是为了[你可以用它做的所有酷东西](http://hackaday.com/2012/04/04/board-games-over-ip-means-telepresence-chess/)。

[https://www.youtube.com/embed/0PWE2QHIXdk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0PWE2QHIXdk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

*在欧洲的一些地方，用 H 表示 B 的键并不罕见。在这个系统中，Bb 的键标为 B and B 是 h