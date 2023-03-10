# 视差推进器 1 开源

> 原文：<https://hackaday.com/2014/08/07/parallax-propeller-1-goes-open-source/>

![OpenPropellerProject](img/c6cf6ace8e5513873ae31219f5eb61db.png) ![OpenSourceProp1Banner](img/4e6eb0cf5b7c6ec9d883915c8639fdb7.png)

Parallax 已经通过[向其 Propeller 1 处理器](http://www.parallax.com/microcontrollers/propeller-1-open-source) (P8X32A)发布源代码来拥抱开源硬件。由[Chip Gracey]设计并于 2006 年发布的 32 位八进制核心推进器已经建立了一个忠实的粉丝群。这些粉丝中的许多人已经为 Propeller 创建了开发工具，从库到[语言端口](https://sites.google.com/site/propellergcc/)。[Ken，Chip]和整个 Parallax 团队已经决定通过向 Propeller 发布整个源代码来支付它。

源代码在 Verilog 中，在 [GNU 通用公共许可证 v3.0](http://www.gnu.org/copyleft/gpl.html) 下发布。Parallax 所做的不仅仅是将 8 年前的文件丢到野外。使用两种不同的目标板在 Altera Cyclone IV 上实现设计所需的所有配置文件也包括在内。 [DE0-Nano](http://www.parallax.com/product/60056) 是低成本选择。 [Altera DE2-115](http://www.parallax.com/product/60050) 开发板更贵，但它也可以运行即将推出的 Propeller 2 设计。

该版本还包括用于引导、运行 cogs 和 SPIN 解释器的 mask ROM 的源代码。【芯片】最初[在 2008 年](http://forums.parallax.com/showthread.php/101483-Propeller-ROM-source-code-HERE)发布这个代码。这些文件包含对 PNut 的引用，PNut 是 Propeller 的原始代码名。

我们很高兴看到 Parallax 迈出这一步，并迫不及待地想看看社区会做出什么样的修改。不是 Altera 的粉丝？没问题——只需拿起源代码、您最喜欢的 FPGA 工具，就可以开始使用了！渴望记忆？再加点就好了。8 个齿轮不够吗？增加到 16。唯一的限制是你的想象力和你的目标设备的资源。

对真正的螺旋桨黑客感兴趣吗？如果你在拉斯维加斯，你很幸运。参加 DEFCON 22 的近 14，000 个徽章中，每个徽章上都有一个螺旋桨。当你在那里的时候，留意麦克和黑客帽！