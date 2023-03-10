# 升级那台廉价的激光切割机！

> 原文：<https://hackaday.com/2014/08/13/upgrade-that-cheap-o-laser-cutter/>

激光切割机可能是黑客空间工具库中最有用的工具之一，只有 3D 打印机和数控铣床可以与之匹敌。问题是它们很贵——除非你能从中国买到便宜的小玩意！不幸的是，物有所值。幸运的是，尽管它们升级起来并不困难！

[Dan Beaven]刚刚完成升级他的 40W CO2 激光器，以使用 Arduino Mega 2560 和 RAMPS 1.4 想要分享他的知识，他发布了一个指南来帮助其他人做同样的事情。升级本身并不困难，尽管布线可能有点乱。将来[Dan]希望设计一种带有所有连接器的 PCB，这样就像把它插到斜坡板上一样简单。

为了控制激光，他使用了兰辛制造商网络( [GitHub](https://github.com/lansing-makers-network/buildlog-lasercutter-marlin) )为马林电子公司设计的固件。他为自己的目的做了一点修改([谷歌驱动](https://drive.google.com/file/d/0B8S25d-5M3YyNG5pVFoxaVBJNjQ/edit?usp=sharing))，包括一个低输出激光激活信号。用这个硬件设置你的激光很酷的一点是你可以在 Inkscape 中使用[一个激光输出插件！](https://github.com/lansing-makers-network/thlaser-inkscape-plugin)