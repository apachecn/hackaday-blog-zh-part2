# 用真火和激光玩太空入侵者

> 原文：<https://hackaday.com/2015/03/25/playing-space-invaders-with-real-fire-and-lasers/>

制作一个太空入侵者游戏是你可以用激光切割机做的最不寻常的事情之一。在观看小飞船爆炸起火的过程中，马丁·雷恩斯福德的改装也是我们见过的最危险的改装之一。

[马丁]总是渴望制作经典游戏的真实版本。由于他的 Whitetooth A1 激光切割机已经包含了所需的大部分移动硬件，更不用说一个真正的高功率激光器来“皮尤皮尤”，他决定这是这样一个项目的完美起点。游戏是向下看着切割机进行的，因为激光当然是朝那个方向发射的，但是一个基本的网络摄像头安装在激光组件上，这样你就可以在计算机屏幕上以正确的视角观看游戏。一个 Arduino Mini 负责步进器控制，允许玩家来回慢跑，并用键盘开火。[Martin]为 z 轴整平机增加了一个额外的齿轮，这样它就可以驱动成排的纸张入侵者左右穿过底部。沿着一个修改过的背板，纸夹楔入插槽中，将每张纸条固定在适当的位置。这很理想，因为他们可以很容易地重新加载，不会在使用中致残。

由于激光的热量，一个定位良好的射击可能会用核武器攻击附近的所有入侵者，从而制造出一个戏剧性的地狱并轻松获胜。现在要提高难度，想办法让他们还击…

[https://www.youtube.com/embed/I0yS4JuiVug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/I0yS4JuiVug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果安全更是你的事情，你可以走的路线[太空 Ivaders 时钟](http://hackaday.com/2010/03/05/space-invaders-clock-6-years-ahead-of-pong-clock/)，16×2 [字符显示游戏](http://hackaday.com/2013/02/04/space-invaders-played-on-a-16x2-character-display/)，或在 FPGA 上头对头[。](http://hackaday.com/2012/01/03/two-player-space-invaders-via-fpgas/)