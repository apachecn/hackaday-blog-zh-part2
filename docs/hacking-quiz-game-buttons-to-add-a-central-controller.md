# 黑客问答游戏按钮添加一个中央控制器

> 原文：<https://hackaday.com/2013/07/18/hacking-quiz-game-buttons-to-add-a-central-controller/>

![hacking-quiz-game-hardware](img/ac20b070889b1365b24ac7f914811fc6.png)

上面看到的四个彩色按钮是学习资源做的一个产品。当按下时，它们会闪烁并发出声音，这是为了在教室里玩智力竞赛节目式的游戏。问题是他们没有使用中央控制器，所以由运行游戏的人来判断谁先进来。[Kenny]通过[构建他自己的控制器](http://www.projectnotions.com/electronics/quiz_game_description)解决了这个问题，控制器位于那个黑色的项目框中。

他带了一块 Arduino Uno 板。它适合在项目框中，并没有问题，监测所有的按钮，并在必要时触发它们的声音和灯光。控制器的两侧有两个电话插孔(RJ11 连接器)。他还敲开了每个按钮，在 PCB 上切割了一些轨迹，以便将信号接入他添加到外壳上的连接器。

休息后的视频显示了该系统的运行情况，除了点亮第一个响铃按钮外，盒子上还有 led 指示灯，指示谁是第二、第三和第四名。

如果你不想买纽扣，试着用一些便宜的塑料碗自己做。

[https://www.youtube.com/embed/4cnihVKw_nw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4cnihVKw_nw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)