# 客座博文:黑掉 C128 准将的真实故事

> 原文：<https://hackaday.com/2013/12/09/guest-post-the-real-story-of-hacking-together-the-commodore-c128/>

迄今为止最受欢迎的计算机是 Commodore C-64，在 20 世纪 80 年代总共售出了 2700 万台。那些 8 位“复古”时代几乎没有留下什么，当时一个年轻的长发自学成才的工程师可以通过纯粹的机会和相当大的决心，坐下来使用自动铅笔、一堆数据书和许多纸张从头设计一台计算机。

[![Before Apple there was Commodore](img/af1493481e3e57731ef58a85e4965e8f.png)](https://hackaday.com/wp-content/uploads/2013/12/c-128-1985-ad.jpg)

Behind the C-128 from a 1985 Ad

我的名字叫比尔·赫德，我是一个留着长发、自学成才的孩子，生活在电子世界里，梦想着电子产品，带着青春的激情，发现自己设计了 Commodore C-128，这是最后一台 8 位计算机，不知何故，它包含了许多家庭计算的第一次。与我一起工作的团队有机会推出最后一台 8 位计算机，前提是我们接受这样一个事实，即无论我们做什么，都必须在 5 个月内完成……赶在 1985 年拉斯维加斯消费电子展(CES)之前。

我们(准将)可以做当时其他电脑公司无法轻易做到的事；我们制造了自己的集成电路(IC ),并拥有当时两大主流 IC；6502 微处理器和 VIC 视频显示集成电路。这种优势将导致一个强大的计算机，但有一定的成本；C-128 的定制集成电路至少在 5 个月内不会准备好，在一个集成电路的情况下，它实际上会被欺骗而无法工作。

在 CES 展之前，在生产之前，在定制集成电路可用之前，为了赶上最后期限，除了黑掉别无选择。我说的黑是指我们必须用 [LS-TTL](http://en.wikipedia.org/wiki/Transistor%E2%80%93transistor_logic#Sub-types) 芯片创建仿真器板，就像 Commodore/MOS 以其闻名的 48 引脚定制 [VLSI](http://en.wikipedia.org/wiki/Very-large-scale_integration) 芯片一样。

[![Commodore C128 aka "the barn door doorstop"](img/368a443979bfab5b05a3a8717d42c972.png)](http://hackaday.com/wp-content/uploads/2013/11/commodore-c128.png)

Commodore C-128, the last mass production 8 bit computer and first home computer with 40 and 80 column displays, dual processors, three operating systems, 128k memory via MMU and one heck of a door stop.

更有趣的是，几周后，处于妄想否认状态的市场部发布了一份新闻稿，保证与 C64 100%兼容。我们争论着问他们(市场部)将如何完成这样一个崇高的目标，但最终还是决定自己开始工作。

随着项目的进展，我们意识到这很可能是 Commodore 的最终 8 位系统。我们开始在 5 个月的时间框架内加入尽可能多的功能。在我们完成之前，我们将拥有双处理器、三操作系统、双显示器(同时支持 40 和 80 列),这是第一台突破 64k 大关的家用电脑。我们开始把 C128 比作装在 5 磅袋子里的 9 磅便便，我们根本装不下 10 磅。我们还开玩笑说出门时要关灯，因为我们知道 8 位时代即将结束。

[![C128-Production-PCB](img/62903ada0cc8b8e025f7284e12bf8895.png)](http://hackaday.com/wp-content/uploads/2013/11/c128-production-pcb.png)

C128 将需要两个全新的 40 针定制芯片；一个内存管理单元(MMU)，一个主可编程逻辑阵列(PLA)，以及古老而可怕的 VICII 视频核心芯片需要重新加工。我们还让芯片人员绑定了一个非常特殊的 48 引脚版本的 6502 微处理器，我们决定使用 Commodore 最新的 80 列芯片，这几乎导致我们错过了 CES。(但那是另一回事了)

[![Commodore C128 with chip emulators acting as place holders for custom chips.](img/5f1ab167eea64ecf58ec2e51cfffde18.png)](http://hackaday.com/wp-content/uploads/2013/11/c128-with-chip-emulators.png)

The initial Commodore C128 with three months to go until CES. Five custom chips have yet to be completed, in the mean time “chip emulators” kept it running enough that the system software could be written.

因此，这就是需要一些严重的黑客攻击的地方；我们需要开始编写软件(一个全新的 Rom 内核和监视器以及一个全新版本的 Basic 结构化命令)，我们需要开始制作 PCB 的过程，我们需要开始调试硬件并理解尝试使用 128k DRAM(是的“k”，不是 m、g 或 t)的含义，这是第一个，也是家用计算机中的第一个 MMU。在此过程中，它变成了一个双处理器系统 6502/Z80，并同时显示 40 列电视和 80 列监视器。家用显示器当时还没有真正出现，我们还指望随着新硬盘的出现，它也能及时出现。

[![Commodore C128 PCB Bottom showing jumpers and "dead bug" IC's.](img/d1b672cb883928788a7e08648373f814.png)](http://hackaday.com/wp-content/uploads/2013/11/c128-underside.png)

Bottom of the prototype C128; Three months until CES and it takes lots of jumpers and chips stuck to the bottom to make it work.

我们最终做的是设计第一个 PCB，采用成品 40 引脚 dip 芯片或 40 引脚仿真器电缆，连接到由 74LS 芯片构建的仿真器板，当与一些相当古怪的[PLA](http://en.wikipedia.org/wiki/Programmable_Logic_Array)(当时的 FPGA)和延迟线以及我们能找到的任何其他东西相结合时，就足够接近于一个定制芯片，程序员可以继续工作。

此幻灯片需要 JavaScript。

我们的构建技术是尽可能多地增加 PCB，然后根据需要增加跳线。虽然在 80 年代的主流是良好的老式绕线，所以我们继续布局牺牲主 PCB 和绕线子组件，以充当定制芯片，有望在几个月内到达。(看着主 PCB 的底部，很难相信在大约 3 个月内，我们将开始几百万的生产。)

此幻灯片需要 JavaScript。

这仅仅是个开始，前面还有一些相当疯狂的组合设备，它们都有两个共同点；当经理们在家睡觉的时候，我们不得不连夜完成所有的修改或修补工作，最终的结果是必须以百万件的数量工作。

在 CES 的最后冲刺阶段，我们在硬件实验室用铝箔吃假日晚餐，使用磁盘驱动器的热量来保温食物，浴室水槽也兼作淋浴。由于长期使用，我的鞋子变得不适合穿了，于是就被丢弃了，结果是一只老鼠在我的脚趾上占据了一席之地。(第一只准将鼠)

我们在展会的前一天晚上在展台组装了设备，Commodore Business Machines (CBM)的员工被要求手动搬运 80 柱芯片，这几乎是展会的一个亮点。移植了 [CPM](http://en.wikipedia.org/wiki/CP/M) 的程序员能够通过编辑软盘上的原始数据来修复最后的 80 个列错误。

此幻灯片需要 JavaScript。

就展会上的产品表现而言，我们做到了。没有失败，没有“蓝屏”时刻，媒体对我们很友好。回到工作岗位后，在经历了这么多月的煎熬后，我们努力思考如何放松下来。人们洗了澡，最终下巴松弛的表情让位于正常的表情。

我们认为我们已经完成了最后一台大型 8 位计算机，我们知道一个时代即将结束，但我们也对 16 位 Amiga 的问世感到兴奋，即使在工程领域有大裁员的传言。没有创始人杰克·特拉米尔的推动，CBM 似乎漫无目的地取消了 next 电脑，LCD 电脑系统几乎没有主要产品的营销。我的感觉是卡梅洛特的时代已经结束了。团队慢慢解散，没有新的挑战将我们团结在一起，我最终在业余时间在新泽西的一个创伤中心工作，因为我对肾上腺素有点上瘾。

* * *

[![The Easter Egg in the Commodore C128](img/f49f1f078ac01de8fe4581c9f28426c6.png)](http://hackaday.com/wp-content/uploads/2013/11/herdware-easter-egg1.png)

The Easter Egg in the Commodore C128

Bil Herd 继续开发高速机器视觉系统，并设计了常见于新车的超声波倒车报警器。在过去的 20 多年里，Bil 一直是一名企业家，并创办了几家小型企业。比尔通过他的网站 c128.com[与旧 Commodore 电脑的收藏家和其他粉丝保持联系，并将很快开设他的新网站 herdware.com](http://c128.com)[T5，该网站将提供开源和教育电子套件。](http://www.herdware.com)

### 复活节彩蛋图片中的 C128 工程队:

Bil Herd:设计师和硬件负责人
Dave Haynie:复杂的时序、PLA 仿真器和 DRAM
Frank Palaia: Z80 集成和 RAM 扩展

Fred Bowen:程序员和软件负责人——核心和监控人员。冯·厄特温:程序员- CPM

Commodore C128 于 1985 年生产，销售了 500 多万台，创造了约 15 亿美元的收入。带有内置磁盘驱动器的 C128D 本应与独立设备同时发布，但 C128D 几年后才投入生产。