# Twitch 玩神奇宝贝:比黄金时间的电视节目更好

> 原文：<https://hackaday.com/2014/02/26/twitch-plays-pokemon-better-than-prime-time-tv/>

当你把一个经典的 Game Boy 游戏、一些胶水代码、一个流媒体视频网站和 1 个互联网放在一起，你会得到什么？ [Twitch 玩神奇宝贝(TPP)](http://www.twitch.tv/twitchplayspokemon) ，这是一个社交实验，成千上万的人“合作”玩一个神奇宝贝红/蓝的游戏。TPP 是由一位匿名的澳大利亚程序员创建的，他喜欢在 [twitch.tv](http://www.twitch.tv) 上的 [SaltyBet](http://www.twitch.tv/SaltyBet) 互动频道。TPP 的创建者决定使用 twitch 自己的基于 IRC 的聊天服务器，而不是使用 SaltyBet 让用户通过外部网站互动的方法。从 [VisualBoyAdvance 开始，](http://en.wikipedia.org/wiki/VisualBoyAdvance)一个流行的基于 C/C++的 Game Boy 模拟器，[TPP 的创造者]开始构建这个系统。[TPP 的创建者]和 python 一起创建了 web-to-emulator 接口。一个 JavaScript 应用程序在屏幕右侧显示实时动作。

游戏很简单——用户在 IRC 或网络客户端输入命令(向上、向下、A、B)。在最初的配置中，命令按照它们到达游戏的顺序进行处理。这个系统一直工作到整个事情像病毒一样传播开来。随着成千上万的人在任何给定的时间输入命令，可怜的“红色”经常会被发现原地打转，或做其他奇怪的事情。这种效果如此引人注目，以至于【Randal Munroe】已经[写了一篇关于它的 XKCD 文章](http://xkcd.com/1333/)。为了帮助玩家通过游戏中一些棘手的部分，[TPP 的创造者]增加了一个游戏模式选择。用户可以玩“民主”游戏，系统会进行几秒钟的投票，然后发布最高票数的命令。原来的一切皆有可能游戏模式改名为“无政府状态”。从一种模式到另一种模式的切换由用户自己实时决定。

我们的读者之一德文也很忙。他写了一篇关于将树莓 Pi 变成专用 TPP 浏览器的教程。我们希望看到一个 TPP [战斗站](http://www.reddit.com/r/battlestations)——一个游戏男孩被修改来显示 TPP，以及当按钮被按下时向 IRC 服务器发送命令。谁会是第一个击败那个黑客的读者？