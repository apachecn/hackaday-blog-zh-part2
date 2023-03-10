# 一边玩口袋妖怪一边给游戏男孩编程

> 原文：<https://hackaday.com/2012/11/24/programming-a-game-boy-while-playing-pokemon/>

我们希望我们的读者熟悉第一代口袋妖怪游戏的大量 ROM 黑客。通过按下特定的按钮序列，有可能复制玩家物品清单中的物品，获得无限的金钱，甚至瞥见难以捉摸的失踪号码。[bortreb]对所有这些黑客都很熟悉，但他从口袋妖怪内部为一个游戏男孩编程的努力是迄今为止最大的口袋妖怪故障。

这种“完全控制”ROM 黑客的灵感来自于[p4wn3r]给人留下极其深刻印象的《口袋妖怪黄》1 分 36 秒的长跑。在[p4wn3r]的运行中使用的技术依赖于这样一个事实，即口袋妖怪黄色中的扭曲点就在游戏男孩内存中的项目列表之后。通过破坏物品列表，[p4wn3r]想出了如何让他家的前门直接弯曲到游戏结束，从而创造出有史以来最快的口袋妖怪速度。

意识到这个 ROM 黑客能够只用玩家的库存来控制 CPU，[bortreb]想看看他能把这个黑客推多远。他最终通过存放和丢弃游戏中 PC 上的项目编写了一个自举程序，然后能够通过按下 D-pad 上的一些按钮，选择，开始，A 和 B 按钮来重新编程游戏男孩。

由此产生的黑客意味着[bortreb]实际上可以制造 Pong、Pacman、MIDI 播放器，甚至是 Pokemon Blue 的副本。在休息后的视频中，你可以看到[bortreb]的速度随着播放《我的小马》主题曲的 MIDI 文件的终曲一起奔跑。[bortreb]手上有一个非常惊人的黑客技术，它真正推动了通过修改口袋妖怪 ROM 可以做什么的定义。

[https://www.youtube.com/embed/p5T81yHkHtI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/p5T81yHkHtI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)