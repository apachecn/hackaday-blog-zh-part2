# 黑客 57–CNC 黑客

> 原文：<https://hackaday.com/2015/07/24/hacklet-57-cnc-hacks/>

每个人的第一个微控制器项目是让 LED 闪烁。它已经成为硬件黑客事实上的“Hello World”。看到你连接的电线和你写的代码一起在现实世界中发生一些事情。LED 不仅仅是屏幕上的像素，它是有形的。从闪烁的发光二极管到让东西动起来只有短短的一步之遥。让东西动起来就像是一种入门药物——它会带来更大的东西，比如机器人、电动汽车和数控机床。计算机数字控制(CNC)是使用计算机控制运动的艺术。该术语通常用于机床，在木材、塑料、金属和其他材料上进行切割、雕刻或其他操作。简而言之，制造更多东西的工具。黑客爱 CNCs 也就不足为奇了。本周的 Hacklet 是关于 [Hackaday.io](https://hackaday.io/) 上一些最好的 CNC 项目！

[![charliex](img/ef9cc2e23b0e5162d7e0f965e77bce59.png)](https://hackaday.io/project/1882) 我们先从【Charliex】和[灰熊 G0704 数控转换](https://hackaday.io/project/1882)说起。[查理克斯]想要一台能铣削金属的结实的机器。他从 Grizzly G0704 开始，它比标准的膝磨机小，但仍然有足够的能力铣削钢。[Charliex]为他的工厂添加了 Flashcut CNC 转换套件。虽然他们称之为“转换套件”，但要让这样的系统运行起来，仍然需要相当多的 DIY 独创性。[Charliex]发现他的锭子跳动远远超出规格，即使对于一家中国工厂也是如此。新的轴承和皮带转换套件使事情变得更加顺利和安静。改装的 G0704 现在整天在查理的车库里切割零件。

[![makesmith](img/abf6fa5800beb9a6685a6c28afa1a09e.png)](https://hackaday.io/project/2750) 接下来是【brashtim】与 [Makesmith CNC](https://hackaday.io/project/2750) 。Makesmith 是(brashtim 的)2014 年 Hackaday 奖的参赛作品。虽然没有获奖，但 Makesmith 确实有了一个非常成功的 Kickstarter，所有机器都在 2014 年 12 月发货。这台机器本身是非正统的。它像大型数控机床一样使用闭环控制，而不是台式设备中常见的开环步进电机。驱动电机是爱好型伺服。我们也不是在谈论标准的伺服系统——[ brash Tim]选择了 microservos。通过使用伺服系统、普通五金店零件和激光切割丙烯酸树脂，[brashtim]降低了成本。这台机器的性能非常好，可以轻松地铣透木头、塑料、泡沫和印刷电路板。

[![reactron](img/ea249461d7f96fe630a4389ae291302e.png)](https://hackaday.io/project/1495) 接下来我们有【Kenji Larsen】带 [Reactron 材料处理器:无线数控铣床](https://hackaday.io/project/1495)。[Kenji]从一个 Shapeoko 2 开始，给它 Reactron 治疗。储备控制器被质子屏蔽所取代，质子屏蔽通过 HopeRF 无线电模块连接到反应堆网络。套件中包含的仿制旋转工具被 DeWalt DW660(用于重型作业)或更安静的 Black and Decker RTX-6 所取代。一个安装在工具上的内窥镜监视着工作。[Kenji]将整个磨机安装在一个定制的泡沫和 Roxul 绝缘外壳中。外壳可以隔音，但也能保温。[Kenji]计划增加一个热交换器来保持物品凉爽，同时保持店里相对安静。

[![cnc2](img/6a66f6f96ec8b4933ad47d1fc4081fac.png)](https://hackaday.io/project/4937) 终于我们有了一台【hebel23】带[的 DIY 复用胶合板数控路由器](https://hackaday.io/project/4937)。[hebel23]想要在预算范围内建造一台大型机器——特别是 400 x 600 x 100 mm 的工作区域和 800 欧元的预算。顾名思义，[hebel23]用桦木胶合板作为机器的框架。他选择了高质量的胶合板，而不是大盒子商店里的廉价材料。这给了机器一个稳定的框架。机器的移动部件也很好——滚珠丝杠、直线轴承和良好的步进控制器。步进电机本身是 NEMA-23 单元，这应该给数控切割木材，塑料，甚至光切金属足够的权力。[hebel23]在他的 CNC 的小细节上花了很多时间，比如添加一个紧急停止开关和一个钢丝链，以防止他的龙门架控制线缠绕在工件上。最终的结果是一台 CNC，在任何人的车间里看起来都很棒。

如果你想要更多数控的好处，看看我们全新的[数控项目清单](https://hackaday.io/list/6906-cnc-projects)！我错过你的项目了吗？不要害羞，只要[在 Hackaday.io](https://hackaday.io/adam) 上给我留言。这就是本周的 Hacklet，一如既往，下周见。同样的黑客时间，同样的黑客频道，带给你最好的 [Hackaday.io](https://hackaday.io) ！