# TP-Link 路由器变成了 DALI 自动照明控制器

> 原文：<https://hackaday.com/2013/06/01/tp-link-router-turned-into-a-dali-automated-lighting-controller/>

![dali-control-in-tplink-router](img/936d1904e87aa998545038144522fb21.png)

Shackspace 的成员继续围绕微型 TP-Link 路由器进行令人印象深刻的黑客攻击。这一次[Timm]在路由器外壳中硬塞了一个 DALI 控制器[。我们不记得以前听说过这个协议。](http://shackspace.de/?p=4099)[数字可寻址照明接口](http://en.wikipedia.org/wiki/Digital_Addressable_Lighting_Interface)是商业照明的控制网络。这样，负责管理大型建筑的人可以在晚上关掉所有的灯(仅举一个例子)。Shackspace 的新房间的灯里有这种类型的控制器。

进入路由器的两条棕色电线构成了 DALI 系统的数据总线。它连接到使用 Atmel AT90PWM316 微控制器的附加 PCB。该芯片是专门为 DALI networks 设计的，这使得项目的其余部分变得非常容易。它跟灯说话，路由器跟它说话，鲍勃是你的叔叔，你有网络控制照明。在一个足够大的建筑里，你可以玩俄罗斯方块。

如果你想知道。是的，这个项目已经被添加到他们的 TP-Link 固件生成器中。