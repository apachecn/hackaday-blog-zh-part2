# 教电脑玩马里奥…似乎是通过巫毒教

> 原文：<https://hackaday.com/2013/04/14/teaching-a-computer-to-play-mario-seemingly-through-voodoo/>

有些人知道[汤姆·墨菲]是[汤姆·墨菲七世博士]，这次黑客攻击表明他赢得了这些荣誉。他决定试试能否教电脑在超级马里奥兄弟中获胜。但是他用了一种我们敢打赌 99.9%的读者首先会想到的不同的方式。这个游戏不关心马里奥，能量，甚至不关心敌人。它只是简单地看一下表明你在游戏中表现良好的指标，即分数和世界/级别。

上面的链接包括他的白皮书，但我们认为在尝试解决这个问题之前，你应该先看看 16 分钟的视频(休息之后)。在剪辑中，他用外行人的术语解释了这个过程，这是目前为止我们唯一真正理解的部分(因此在标题中提到了伏都教)。他的程序使用试探法来组装一组不断进化的控制器输入，以推动分数不断提高。换句话说，他的软件一遍又一遍地玩游戏，学习哪些控制器输入组合会导致成功，哪些不会，而不是跟随像人类一样玩游戏的[扫雷解算器](http://hackaday.com/2012/12/24/how-to-write-your-own-minesweeper-solver/)或[宝石迷阵闪电战机器人](http://hackaday.com/2011/07/30/bejeweled-blitz-bot-makes-your-high-score-look-just-sad/)的脚步。右边的图片是它学习进度的图表。很有道理，是吧？

[https://www.youtube.com/embed/xOCurBYI_gY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xOCurBYI_gY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/programming/comments/1c4m47/video_computer_program_that_learns_to_play/)