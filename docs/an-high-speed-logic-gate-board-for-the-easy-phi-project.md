# Easy-Phi 项目的高速逻辑门板

> 原文：<https://hackaday.com/2014/04/24/an-high-speed-logic-gate-board-for-the-easy-phi-project/>

[![](img/7bdadef2279ac2112152982bf24c9bb0.png)](http://hackaday.com/wp-content/uploads/2014/04/logic_gate_board.jpg)

不久前，我向你们展示了 Easy-phi 项目，该项目旨在为业余爱好者构建一个简单、廉价但智能的基于机架的开放硬件/软件平台。在这个项目中，您只需在一个机架上添加卡片(如上图所示)即可实现您想要的功能。

在过去的几个月里，我的团队已经完成了几种不同电路板的设计和生产，所以我将在接下来的几周内开始展示它们。今天我向大家展示的是[高速逻辑门板](http://www.limpkin.fr/index.php?post/2014/04/30/Easy-phi-project%3A-High-Speed-Logic-Gate)，这是一个量子物理学家要求的 easy-phi 模块，可以以< 2GHz 的速度执行逻辑和/或功能。这篇技术性很强的文章主要讨论高速信号给原理图设计带来的限制，同时也涉及用于 HS 信号端接和监控的技术。然而，我希望它能让我们的读者对高速系统的内部有一个很好的了解。该板使用的所有文件都可以在官方 [GitHub 库](https://github.com/easy-phi/main/tree/master/Modules/High-speed%20Logic%20gate/Current%20Version/github)找到。