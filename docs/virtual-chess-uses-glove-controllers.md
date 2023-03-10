# 虚拟象棋使用手套控制器

> 原文：<https://hackaday.com/2012/12/11/virtual-chess-uses-glove-controllers/>

![chess-using-glove-controllers](img/3293102f298145b3769b6cd9540f8d4d.png)

[看看上面正在进行的象棋比赛](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2012/oaq3_cig23_rk447/oaq3_cig23_rk447/index.html)。这是一个虚拟游戏，每个玩家用一只手套作为控制器。或者当然游戏棋盘和棋子从这个图像中消失了。它们显示在电脑显示器上，双方都能看到。

硬件相当简单，我们认为这将是一个伟大的项目来挑战你的微控制器技能。每只手套上都有一个加速度计，在食指和拇指上还有一圈铜箔。一个 ATmega1284 监控两只手套。加速度计数据用于在屏幕上移动鼠标光标，而触点用于抓住或释放游戏棋子。游戏棋盘和棋子使用 MATLAB 显示，控制器命令通过 USB 连接输入。

如果你更喜欢构建一个机械化的游戏[，看看这对网真棋盘](http://hackaday.com/2012/04/04/board-games-over-ip-means-telepresence-chess/)。

[https://www.youtube.com/embed/FAWJ1L3_M4U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FAWJ1L3_M4U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)