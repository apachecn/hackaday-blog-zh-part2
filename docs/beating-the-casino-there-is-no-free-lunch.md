# 击败赌场:没有免费的午餐

> 原文：<https://hackaday.com/2015/08/31/beating-the-casino-there-is-no-free-lunch/>

当你是一个硬件家伙，你生活在一个危机时刻，迟早你会发现自己为一些赌场设备公司工作。你成为了一个圈内人，了解了很多他们的伎俩。我已经和那家企业接触了大约 30 年。我为目前正在使用的赌博机做了很多项目，我和赌场的人有很多接触，包括老板和赌徒。

现在我确信你期望我告诉你他们用什么样的伎俩来让你花钱。我会的:没有什么技术诀窍。这不是因为他们是老实人，而是因为他们不需要。数学和心理学做所有的工作。

赌博的风险有回报吗？从数学的角度来说，不会——但这取决于你自己的决定。有一件事是肯定的——无论你是否决定赌博，了解这些赌场机器是如何运作的都是有益的。了解你的敌人。

## 典型赌徒的财务图表

让我们看看在一个典型的吃角子老虎机游戏过程中，赌徒的钱是如何波动的。玩家从 S 开始，通常会有小输，但也会有小赢。有时他会赢得更大的金额，但从长远来看，很明显他正在走向零。这只是一个普通游戏的例子，虽然它不会总是这样，但大多数时候会这样。即使他在一个好的日子里赢了，你也可以简单地缩放相同的图表，并将其应用于他生命中更长的一段时间。

![diag1](img/b685d8b9a6dc035a46c7cec6c46da6ad.png)

赌博机器不会提前“画”出这个图，它甚至不会提前一步计划。没有“秘密计划”，只有简单的算术规则来决定收益的多少，或者在某些情况下，决定获胜的概率。当你把它和随机化过程结合起来，你就得到图表，仅此而已。

从形式上来说，比赛是公平的，也是符合规定的。对双方来说，赔率都是公平的，尽管赌场有一点优势，因为它有费用要支付。

如果游戏是真正公平的，那么为什么有那么多富有的赌场老板，甚至更多贫穷的赌徒？没有什么特别的原因，我们都知道一小部分投入到了赌场，我们都同意这是公平的，但这正是数学和心理学发挥作用的地方。首先，每当玩家按下按钮，或者运行新的循环，无论他玩什么游戏，都会从他那里拿走“少量”的钱。这种循环可能只持续几秒钟，因此累积效应可能非常显著。如果你是游戏开发工程师，请记住，如果游戏速度更快，赌场老板会更喜欢它。猜猜为什么？

![diag2](img/ec8c9bf1991b9660bb4eabf0aaa27191.png)

这张图说明了为什么游戏必须要快。让我们假设，在第一次假设博弈之后，输/赢的机会类似于高斯分布。最大的赔率在高斯钟形曲线的中心，但也有小的机会获得大的收益或大的损失，特别是如果玩家有冒险的风格。重要的是要注意，图表是不平衡的，因为丢失的可能性稍高。

左图只对第一局有效，之后玩家再按下按钮。五场比赛后，累积效应变得可见，30 场比赛后一切都清楚了。即使在那之后，游戏还会继续，直到系统崩溃，这通常意味着玩家这边已经没钱了。他知道这是怎么回事，但他一直玩到最后。这还公平吗？我有疑问。

很久以前，我被要求对一个老的扑克电子游戏进行修改。在每一轮成功后，玩家可以执行一个动作，他有 50-50 的机会加倍或输掉他最后的赢款。他必须按下两个按钮中的一个，猜测卡片(背面可见)是小于还是大于 7。我必须对一个 8 位 6502 微处理器的固件进行逆向工程，所以我必须反汇编代码，看看它是如何工作的。我真的很惊讶地看到，在那一刻，卡号仍然不存在——相反，有一个决定，由系统，玩家是否会赢或输！当玩家按下按钮时，卡号被随机生成(在期望结果的范围内),其位图被写入视频存储器。

我目睹了很多球员，当他们将要输的时候，大喊“该死的，我为什么不按…”。我怎么能告诉他们结果会是一样的呢？

## 赌博心理学

每个在赌场呆过一段时间的人都知道，每台赌博机对赢的反应都非常戏剧化，有响亮的音乐和叮当的声音，每一次输都是安静而迅速的，然后是下一场游戏的邀请。大赢的记住了，经常提起很久，输的忘记了。赌博有回报的假象就是这么制造出来的。这个特征被称为*选择性阐述*，它起着重要的作用，不仅在赌瘾上，也在对超自然、通灵能力、占星术、骗术等等的信仰上。

再看第一张图表。有很多好赢的，标着笑脸。每一个都给玩家带来了快感和希望，只有最后一个给他带来了不满。收益是巨大的，出乎意料的，损失是小的，渐进的——你可以说它们几乎不明显。感觉到很多快乐而只有一点点不舒服，这值得吗？这要由赌徒来决定，但这种错觉显然起了作用，因为他从不认为自己是个失败者，即使当他失去了一切。他知道，一旦他得到更多的钱，他会再来，这将是，毫无疑问，他的幸运日。

看着第一张图表，很难抗拒这种感觉，他应该在他的信用是开始时的两倍时结束游戏。回过头来看，这对于玩家来说也很清楚，但这是一个激动的时刻——他得到了他的血清素(快乐激素),当你必须做出一个明智的决定时，情绪高涨并不是一件好事。这导致了他意识的缩小，他把它体验为自己的“幸运时刻”，这是每个赌徒的陷阱。你有没有想过为什么赌场里没有日光也没有时钟？整个世界的时间都停止了，你要做的就是赌博。

很少有玩家能判断何时戒赌是明智的。刚开始进展顺利，新的收获就在眼前，真的很难停下来。除了没钱之外，只有一种情况下玩家会有停止游戏的想法:当他获得超级头奖时。然后是享受的时候，不是玩的时候。他拿了钱走了，但总有一天，他会来拿更多的钱。当然，他下了更大的注，因为他现在是高赌注玩家。不归还他赢得的一切，他是不会罢休的。

最近，我在马其顿南部一家不错的赌场安装了一些设备，那里有很多希腊游客。当一名希腊妇女赢得 24，000 英镑的€累积奖金时，每个人都很兴奋。我的第一个想法是，如果她足够聪明，她会离开，永远不再踏进赌场一步。当我两周后再次来到那里时，赌场的工作人员告诉我，她已经“归还”了大约一半的金额。又过了两周，她的计数远低于零。

## 我不迷信，它会带来厄运

大多数(如果不是全部的话)赌徒都很迷信。他们有他们的幸运日，幸运的衣服，幸运的号码，无论什么——总有一个明显的原因来决定输赢。因此，第一个图表中的胜利是因为一名球员的幸运 t 恤(蓝色，他的幸运色)，但当他无意中交叉双腿时，一切都变得糟糕。此外，在进入赌场之前，他不能忘记明天做他的幸运仪式。

迷信通常意味着不擅长数学和逻辑，尤其是批判性思维。毕竟，如果热情的赌徒知道如何批判性地思考，他们可能永远不会踏入赌博的世界。

作为概率论中的文盲，赌徒们经常成为被称为“赌徒谬误”的逻辑悖论的受害者，他们期望一系列相同的结果会对应相反的结果。例如，如果一个轮盘赌轮盘连续多次落在黑色上，他们希望它落在红色上。有趣的是，宾果和彩票游戏的玩家经常得出相反的结论——如果某个数字比其他数字更频繁地被抽取，这意味着它注定会被抽取，并且应该被更多地使用。

这两种“思想流派”互相排斥，当然都是错误的。如果轮盘赌轮 10 次落在红色上，下一轮落在红色或黑色上的几率完全相同。正如数学学家所说，骰子没有记忆。

许多试图黑掉彩票、赌场或在线游戏的赌徒创建了许多下注系统。对他们来说不幸的是，大多数游戏中的数学算法非常简单，这使得他们很难找到任何可以被赌博策略利用的弱点。

当一个赌徒赢了一大笔钱，这离“超级 bingo”只有一步之遥，这一步看起来比它实际上要小得多。例如，如果他玩 7/39 乐透 ( [翻译为](https://translate.google.com/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=https%3A%2F%2Fwww.lutrija.hr%2Fcms%2Floto7od39&edit-text=))并且有 6 个号码匹配，他会觉得自己非常接近终极大奖，但事实上他离得非常远。有 224 个可能的 6，只有一个 7，这是 99.6%对 0.4%。看起来不再那么“近”了！

人脑擅长在许多现实生活情况下做出快速估计，但当涉及到概率论和大数时，它很容易被愚弄。如果你把它和选择性的阐述结合起来，就会导致非常糟糕的评价，进而导致糟糕的决策。组织任何类型赌博活动的人知道这一点，他试图传播关于赢家的故事，但从不提及数千甚至数百万人的钱一无所获。

## 你能黑进赌场吗？

但是，永远不要说不！众所周知，这里所说的例外是 21 点游戏。玩家可以使用策略在游戏中获得一定的优势，但它假设使用非法设备或特殊的心理技术，包括强化记忆和计算，有被永久列入黑名单的风险。一些玩家也在网游中猎取 bug，但更有可能的是实验会损失很多钱，而不是找到一个可行的弱点。

你认为你能黑进赌场吗，即使是网上的？要做到这一点，准备好智胜一个高薪专业团队，他们花了大量的时间和资源来确保你不会。你可能不会因为一个简单的项目而得分，但如果你有扎实的知识背景，并花大量时间研究这个问题，你可能会有机会。

最容易受到攻击的赌博机器是那些带有机械随机发生器和自动阅读的机器。光学阅读器(条形码或带有 OCR 软件的相机)可能会被过量的光(改良的激光指示器或类似设备)欺骗，而 RFID 阅读器可能会被 125 KHz 或 13，56 MHz 的干扰器欺骗。任何知道如何使用它的人，如果他不喜欢刚刚抽出的球或骰子，都可以用这个装置破坏机器。我见过很多赌场没有配备可以防止这种攻击的传感器。无论如何，以原始形式使用这个想法太危险了，所以攻击者需要仔细考虑他的方法，当然，还要留意监控摄像头。

阿尔伯特·爱因斯坦曾经说过:“没有人能在轮盘赌中获胜，除非他趁赌台管理员不注意从桌上偷钱。”他可能是有史以来最伟大的黑客，但每个人都有犯错的权利。

[插图由鲍勃·日夫科维奇绘制]

* * *

沃佳·安东尼克是一名自由微控制器工程师。他的第一个基于 Z80 的微处理器项目可以追溯到 1977 年，就在第一个英特尔 4004 出现的几年后。他用笔和纸手工组装固件。1983 年，他发表了自己的原创 DIY 微型计算机项目，名为 [Galaksija](http://en.wikipedia.org/wiki/Galaksija_(computer)) ，由前南斯拉夫大约 8000 名爱好者建造。到目前为止，他已经发表了 50 多个项目，大部分都是基于微控制器的，并且都是在公共领域发布的。