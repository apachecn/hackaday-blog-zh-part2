# 开源触觉套件旨在使力反馈大众化

> 原文：<https://hackaday.com/2015/01/21/open-source-haptics-kit-aims-to-democratize-force-feedback/>

如果你一直关注增强和虚拟现实新闻，你会记得空间触觉反馈设备并不是开创性的新技术。但是，您还会记得，专业系统是出了名的昂贵——大约几千美元。研究生[乔纳斯]、[迈克尔]、[乔迪]和他们的教授[伊娃-洛塔]组成了设计团队，旨在通过为你提供可以在家里制作的设计[来弥合巨大的价格差距](http://woodenhaptics.org/ "a design that you can build at home")。

快速术语潜水:空间触觉设备是一种物理操纵器，它通过力反馈实现虚拟空间的探索。用户抓住“操纵装置”(手柄)，并在由设备的物理设计所限定的工作区域内移动它。空间触觉设备已经存在很多年了，它是告诉用户(外科医生)某种东西(肿瘤)“感觉如何”的极好工具

在我们的案例中，这种触觉设备是一个双连杆、双关节系统，以基站为基础，通过伺服电机和张紧的钢丝绳提供力反馈。操纵器本身支持末端执行器的 3 自由度运动(平移，但不旋转)，该运动由放置在所有关节上的编码器跟踪。为了实现反馈，接头与电缆驱动传输接合。

设计团队对迭代原型并不陌生。来自斯坦福大学的一门课程 [CS235](http://www.stanford.edu/group/sailsbury_robotx/cgi-bin/salisbury_lab/?page_id=1041) ，旨在向非修修补补者传授原型制作技术，设计师们从这门课程中汲取了许多技术，以提供一个功能齐全且可重复的设置。事实上，很明显，设计者对他们的系统物理有很强的理解，他们利用了一些我们无法立即直观感受到的技巧。例如，他们不是将电缆刚性地固定到电机轴上，而是简单地将电缆缠绕在轴上仅仅 5 圈，使得摩擦力大大超过否则会导致滑动的阈值量。他们还选择胶合板——不一定是因为它的价格——而是因为它作为一种坚硬的分层复合材料的功能，使其成为刚性传递力的理想“杠杆臂材料”。

关于他们设计的完整分类，请看他们的[会议论文](http://woodenhaptics.org/woodenhaptics-tei-2015-paper.pdf "conference paper") (PDF)，其中他们评估了他们的设计技术并概述了正向运动学。他们还提供了一份非常全面的[材料清单](https://docs.google.com/spreadsheets/d/1TH7dbyf5o4HNyC1T4yamnJe4fJo1p8FN_N7bmFLR3ZI/edit#gid=0)(谷歌电子表格)。最后，作为名正言顺的开源硬件，他们已经将他们的[控制软件和 CAD 模型](https://github.com/WoodenHaptics/TEI_2015/ "control software and CAD models")打包到 github 存储库中，这样你也可以跳入高质量力反馈模拟的世界，而不必为一个专业系统支付两万美元。

[通过 [2015 有形嵌入和具体化会议](http://www.tei-conf.org/15/)

[https://www.youtube.com/embed/jc56gvltLbA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jc56gvltLbA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)