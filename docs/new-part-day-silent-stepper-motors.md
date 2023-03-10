# 新零件日:静音步进电机

> 原文：<https://hackaday.com/2015/01/24/new-part-day-silent-stepper-motors/>

进入家庭和学校的第一批受欢迎的打印机是 Apple Imagewriters 和其他速度极慢的点阵打印机。现在每个办公室都有一台安静、快速、高质量的激光打印机，这是点阵技术无法比拟的。

如果你没有注意到，3D 打印机非常慢，非常吵，每个人都期待着有一天可以在短短几分钟内打印出高质量的 3D 物体。我们还没有达到真正安静的步进电机成为可能的地步，但是有了 Trinamic TMC 2100 T1，我们正在达到这一步。

你会在 RepRaps 和其他 3D 打印机中找到的大多数步进电机都是基于步进电机驱动器的 [Allegro A498X 系列](http://www.allegromicro.com/en/Products/Motor-Driver-And-Interface-ICs/Bipolar-Stepper-Motor-Drivers.aspx)，无论它们是在像“[Pololu](https://www.pololu.com/product/1182)这样的分线板上，还是集成在像 [RAMBO](http://reprap.org/wiki/Rambo) 这样的控制板上。Trinamic TMC2100 与 A498X 的*逻辑*兼容，但与*引脚*不兼容。对于 99%的人来说，这不是问题:驱动器通常焊接在分线板上。

Trinamic 芯片的几个特点使其成为一款有趣的芯片。最受关注的功能是一种叫做 stealthChop 的模式。当电机以中速或低速运行时，电机将完全静音。是的，这意味着步进电机音乐将很快成为历史。

然而，这种 stealthChop 模式大大降低了电机可以提供的扭矩。3D 打印机在打印时会以相当快的速度绕着相对较重的轴旋转，这种电机驱动器只能在低速或中速下使用。

TMC2100 的 spreadCycle 功能是您想要用于 3D 打印机的功能。这种模式在电机的每一步使用两个“衰减阶段”,以提高驱动器的效率。3D 打印机中的马达有时会变热，尤其是当它们运行得很快时。更高效的驱动器可以减少热量，有望实现更可靠的电机控制。

除了一些新的操作模式，TMC2100 还有一个非常有趣的特性:诊断。有专门用于通知输出短路、高温和欠压情况的引脚。这是通常的步进驱动器所没有的，如果像这样的功能能够进入 3D 打印机控制器板，那就太好了。我敢肯定，我不是唯一一个收集油炸 Pololu 驱动程序的人，在控制板中正确地实现这些诊断引脚本来可以拯救那些驱动程序。

这些驱动程序现在有点难找，但是 Watterott 已经将其中的一些组装到 Pololu 兼容的包中。[Thomas Sanladerer]也对这些车手进行了精彩的拆解。你可以看看下面的视频。

[https://www.youtube.com/embed/g6Bxoqr8QlY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/g6Bxoqr8QlY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)