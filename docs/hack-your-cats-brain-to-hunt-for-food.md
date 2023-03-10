# 破解你的猫的大脑来寻找食物

> 原文：<https://hackaday.com/2015/08/08/hack-your-cats-brain-to-hunt-for-food/>

由[本·米伦]设计的这个[猫喂食器项目](http://benjaminmillam.com/cat-geek/monkey-the-cat-hunts-for-dinner/)非常吸引人。这一切都始于他读到一个可能的解释，为什么家猫似乎没有必要探索家里的相同区域。一种可能是这只猫在练习它的移动捕猎技巧。那只猫四处嗅着，希望能惊起它的猎物，抓些东西当晚餐。不幸的是，家猫并不经常满足这种原始的欲望。[Ben]思考了这个问题，提出了一个非常有趣的解决方案。其中包括黑进一个电子喂猫器，以及黑进他的猫的大脑。

最重要的是。点击休息时间观看演示视频，观看[本的]猫寻找猎物。然后惊奇地看着猫把它的赏金带回喂猫器，用它来交换一些真正的食物。

[https://www.youtube.com/embed/rTY8MAjd3_k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rTY8MAjd3_k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[Ben]首先想到在房子周围藏几碗食物让他的猫找到，但在想象了他必须处理的未来蚂蚁踪迹后，他很快打消了这个想法。相反，他认为最好藏些其他的东西。一种既不会吸引害虫，也不会随时间变坏的物品。问题是，他的猫必须知道首先取回物体，然后将它放回特定的地方，以获得食物作为奖励。这就是猫黑客的用武之地。

[本]开始用响片法训练他的猫。毕竟，如果猫不能被训练，建立一个复杂的喂食机制是没有用的。他训练这只猫执行两种不同的行为，一次一点点。第一个行为是教猫捡球。这种行为被分解成六个微小的行为，这些行为将被慢慢地连接在一起。

*   看这个球
*   接近球
*   嗅球
*   咬住球
*   捡起球
*   捡起球并保持几秒钟

[本]会按下遥控器，在看到每个行为的预期步骤后立即奖励他的猫。一旦猫有规律地执行了那一步，奖励就被取消，只有当链条中的下一步被执行时才会给猫。最终，猫学会了整个步骤链，导致了期望的行为。

接下来，[本]必须教他的猫关于目标区域。这是一个单独训练的行为，分为以下三个步骤。

*   看目标区域
*   接近目标区域
*   嗅目标区域

一旦猫学会了这两种行为，[本]必须以某种方式将它们联系起来。这一部分需要一点运气和大量的坚持。[本]会把球放在目标区附近，但不要太近。然后，只有当猫捡起球并开始向目标区域靠近时，他才会奖励他的猫。这里有一些风险，如果猫根本不朝着目标区域移动，你就冒着熄灭旧行为的风险，它们将不得不重新学习。幸运的是，[本的]猫足够聪明，能够发现它。

随着猫适当的训练，是时候建立猫喂食器。[Ben]使用了一种现成的叫做超级喂食器的电子喂食器作为他项目的基础。进料器由连接到 Arduino 的继电器控制。Arduino 还连接到一个 RFID 阅读器。每个塑料球里面都有一个 RFID 标签。当猫将球放入目标区域时，读取器检测到球的存在，并触发继电器几秒钟。该系统还包括一个 315 兆赫无线接收器和遥控器。这使得[Ben]可以在需要的时候手动分发一些猫粮。

现在，每当猫饿了，它就可以用这些原始的本能去寻找食物，而不仅仅是随意地把食物递给它。

[谢谢丹]