# 可编程逻辑 I–PLA/PAL

> 原文：<https://hackaday.com/2014/06/24/programmable-logic-i-plapal/>

[https://www.youtube.com/embed/2u77sAfka4w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2u77sAfka4w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
[![C64-B](img/b398ad1c782c2e379fac1fa03aff3850.png)](http://hackaday.com/wp-content/uploads/2014/06/c64-b.png)

是的，我仍然有点生气，因为竞争仍然存在，而我们没有，我说的“我们”是指 Commodore Business Machines (CBM)。正是 Commodore 拥有 C64 中最受欢迎的家用电脑(2700 万台)，毕竟是 MOS 工程师团队有了用 12 平方英寸的 PCB 制作“微型”处理器的想法。

[![MOS Technologies logo and address](img/afa6700589ffe61510d4b77b87574ba0.png)](http://hackaday.com/wp-content/uploads/2014/06/images.jpg)

MOS Technology in King of Prussia/Norristown

当然，他们当时确实在摩托罗拉工作，而“Mot”不想与馅饼盘大小的处理器的利润率下降有任何关系。当然，MOS 被摩托罗拉起诉了，但这只是 MOS/CBM 的一个普通周二。我绝对相信 CBM 收购了 MOS Technologies 芯片代工厂，因为我们可以一起制造自己的处理器、图形芯片、声音芯片、内存控制器和可编程逻辑。

有了这个武器库，我们不必像其他公司那样做出妥协，例如符合工业标准 6845 的总线规范，或者在定制的额外引脚可以工作时增加额外的逻辑。我们也可以制作[精灵](http://en.wikipedia.org/wiki/Sprite_(computer_graphics) "Sprites, I mean Movable Object Blocks.")。

[![6502 Design Team](img/7a7a65ea3f180f9461a4638ff80852ec.png)](http://hackaday.com/wp-content/uploads/2014/06/mos_technology_6502_computer_chip_cpu2.gif)

6502 Design Team (EE Times 1975, archive.archaeology.org)

我们在设计时不得不做出的妥协是成本，我指的是在生产过程中找到节省 1 美元(1 美元)的方法来节省数百万美元的成本。有一天，我从一个变压器里敲了 0.90 美元，由于兴奋，我无法集中精力。

降低成本是一个苛刻的情妇，但你不能只是做一点点的时候，或者只有当你想。将任何东西乘以一百万的心理练习总是存在，这使得买午餐变得很难——我会在计算一百万份金枪鱼三明治的成本时排队买午餐

为了抵消严格的成本控制，我们有大量的折扣。打电话给当地代表说我们正在设计最近的 16kx4 DRAM 被称为“电话”,不可避免地门铃会在挂断电话 2 分钟后响起。

在一次罕见的事件中，当杰克·特拉米尔先生辞职后，我们失去了管理，后来他去了 T2 雅达利公司——想象一下博格人知道 Cpt 的一切。皮卡德有。在“没有管理”的时期，发生了几件事:现场消费的啤酒数量激增，工程部门设计了一台计算机来填补空白，至少在一段时间内没有管理或营销的指导。

这意味着设计最终来自一张网格纸，而不是几十次讨论客户焦点和一百万份金枪鱼三明治成本的会议。购物清单包括一个内存管理器和迄今为止我们做过的最大的计划。需要注意的是，现阶段芯片设计没有人说“不”或者“我们做不到”。那是因为我们还不知道。但是，如果提出请求的工程师不想以后被物理定律所束缚，他/她最好将请求保持在“几乎可行”的范围内。

在 Commodore 64 中，有一个模仿 Signetics 82S100 的 PLA，Signetics 82s 100 是一种用于编程简单 AND-OR 阵列的“熔断熔丝”技术。当我说熔断保险丝时，我不是在开玩笑，我的记忆是，部分参数是不要使用过多的功率来熔断保险丝，因为它会“飞溅”。

[![PLA Die C128.com, ](img/7776b20f761c58fc8f8a6f166d8ad475.png)](http://hackaday.com/wp-content/uploads/2014/06/pla-die.jpg)

PLA Die C128.com,

最终，准将和 MOS 技术公司制作了他们自己的 NMOS 版本，我不会说我们复制了 Signetics 部分，我们只是通过显微镜拍摄了许多宝丽来照片，并把它们安装在一块板上。在覆盖层下，我们用扩散层“块”和预欧姆接触代替了两种熔丝，“和”术语“熔丝”和“或”术语。这是一对一的，因此可以将在 82S100 上工作的代码发送过来，然后有人可以运行脚本进行转换。一篇由[Thomas 'skoe' Giesel] [撰写的关于 Commodore C64 PLA 的出色文章，收录在本 PDF 文件](http://skoe.de/docs/c64-dissected/pla/c64_pla_dissected_a4ss.pdf)(此处还引用了[)。](http://www.zimmers.net/anonftp/pub/cbm/firmware/computers/c64/C64_PLA_Dissected.pdf)

[OR 'ing 就像一堆狗，芯片并不关心哪一串术语引起了真实的情况，它只知道是一个或多个引起的。](http://hackaday.com/wp-content/uploads/2014/06/initials.jpg)

[![PLA Worksheet](img/84ffe38af4573e9b959e342dbf729f1f.png)](https://hackaday.com/wp-content/uploads/2014/06/pla-worksheet.png)

Example of the worksheet engineers used to create logic terms.

我们竭尽全力推动这个器件，我要求的是两倍多一点的条件，这意味着两倍大的阵列，有两倍的电阻和两倍的电容。这相当于 RC 分量的 4 倍。除此之外，我也不会对设计师如何在没有告诉任何人的情况下尝试插入更改，并在 CES 开幕前两周将所有输入引脚短路到反向偏置环的细节感到厌烦。简而言之，我们把尽可能多的东西塞进芯片，没有它我们就不会有一台可行的计算机。大批量生产的定价使成本降到了几分几毫，甚至在 NRE 的设计成本高达 250 万美元之后。

[![PLA And Or Array](img/1ae9a988acb1c2ac959c689964a014e6.png)](http://hackaday.com/wp-content/uploads/2014/06/pla4.png)

PLA And Or Array

所以解放军是一个低成本，高回报的打击。我们笑了。然后我们看着留在黑板上的所谓丛林逻辑，眉头紧锁。这组门将是当今可编程逻辑器件(PLD)的主要候选，尤其是在我们试图使 6502 微处理器与 Z80 微处理器很好地配合，同时又不破坏 DRAM 的领域。这对于 FCC 申请的最后阶段也是非常理想的，在这一阶段，你只需要对公告板做最小的可见修改，而不需要重新提交。然而，在 Mudville 没有欢乐，因为 PLD 的价格高得令人望而却步，只有 4-5 美元。大量购买并没有带来大的折扣，只是大的账单和物流问题，比如编程。在这一点上，我得到了一份机密的库存和价格表，并从库存中挑选了丛林逻辑，假设任何一个零件都有几十万个可用。

[![PLD Architecture](img/0586be25d97b8665cabb2cd8c615443b.png)](http://hackaday.com/wp-content/uploads/2014/06/pld-nots.png)

PLD architecture showing registers and feedback.

PLA 的强大之处在于它的速度相对较快，因为内部数组较小，并且增加了寄存器和反馈项，这些都是状态机的组成部分(我们将在稍后讨论 Mealy 和 Moore 状态机。)我相信 CBM/MOS 确实尝试过做一个 NMOS 版的 PLA，但是 NMOS 进程的局限性限制了可用性。在明天早些时候发表的下一期文章中，我将从头到尾讨论更现代的复杂可编程逻辑器件和编程一。现代器件并没有减少门数，而是允许设计人员实现任意数量的宏功能，这种简单的功能无法实现，因为“丛林逻辑”太慢且容易出错。

[![CPLD Device showing assignments.](img/a8867aa356742f1ae53afd07a4a3bbac.png)](http://hackaday.com/wp-content/uploads/2014/06/altera2.png)

CPLD Device showing assignments.