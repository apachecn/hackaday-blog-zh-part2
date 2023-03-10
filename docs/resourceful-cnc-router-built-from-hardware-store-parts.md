# 足智多谋的数控路由器建立从五金店的部分

> 原文：<https://hackaday.com/2015/01/05/resourceful-cnc-router-built-from-hardware-store-parts/>

[siemen]已经带着他的低成本建造的[龙门式路由器](http://www.instructables.com/id/CHEAP-ARDUINO-CNC/?ALLSTEPS)进入了业余爱好 CNC 的奇妙世界。它体现了我们在这里所爱的一切:机智、毅力和结果。[西蒙]利用他在网上冲浪时发现的想法设计了他的框架，它完全是由刨花板制成的。对于线性运动，Y 和 Z 轴依靠滚珠轴承抽屉滑轨，而 X 轴使用管道和滑板轴承配置。NEMA 17 步进电机耦合到螺纹杆移动每个轴。

电子产品被封装在一个漂亮的小项目盒中，其中包含一个 Arduino 和 3 个 Sparkfun EasyStepper 步进电机驱动器。[siemen]还在项目箱上切了一个洞，并安装了一个风扇，以保持那些电机驱动器的冷却。Arduino 与名为 [GRBL](https://github.com/grbl/grbl) 的 CNC 机器控制器一起被刷新。GRBL 将从 PC 发送的 g 代码传送到 Arduino，然后依次将所需的步进和方向信号发送到步进电机驱动器。

总的来说，[siemen]在他的第一个 CNC 项目上做得很好，获得了 200 欧元(240 美元)。他目前正在开发第二版，我们期待着在它完成的时候报道它。如果你喜欢这个项目，你可能也会喜欢这个[木制木刳刨机](http://hackaday.com/2014/07/11/400-diy-cnc-machine-is-surprisingly-simple/)或者这个[螺栓连接的](http://hackaday.com/2011/06/07/diy-bolt-together-cnc-router/)。

![resourcefulcncrouter-mid](img/6fc064b0170c207cfa9a289c78cdcc7d.png)