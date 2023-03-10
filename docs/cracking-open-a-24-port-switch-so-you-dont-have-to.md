# 打开 24 端口交换机，这样你就不必

> 原文：<https://hackaday.com/2013/02/15/cracking-open-a-24-port-switch-so-you-dont-have-to/>

![hp-procurve-ethernet-switch-teardown](img/7ec9f5e72a5f1380682a53bef5fd3021.png)

[Kenneth Finnegan 的]关于这个 [24 端口 HP ProCurve 2824 以太网交换机拆卸](http://blog.thelifeofkenneth.com/2013/02/tear-down-of-hp-procurve-2824-ethernet.html)的帖子读起来很愉快。他正在加州州立理工大学学习网络入门课程。他们的一个实验室包括虚拟机，这些虚拟机同时拍摄数千个新的 MAC 地址。尽管它能够以极快的速度交换数据，但它处理这么多新硬件标识符的能力并不令人印象深刻。他想找出原因，碰巧他家里的零件箱里有一个这样的东西(他指的好像是一个高能 RPG 角色)。

主板分为三个主要部分:电源、开关硬件和使其成为管理开关的处理器。虽然他涵盖了所有这些部分(交换的东西学习起来非常有趣)，但正是处理器部分导致了前面提到的速度下降。这是一个 266MHz 的 PowerPC 芯片，内存只有区区 64 MB。当然，这并不需要更强大，因为来自先前“学习”的 MAC 地址的所有流量都由交换块处理，并且从不触及处理器部分。

不要错过他的帖子的结尾，他讨论了滤波电容和半隔离接地层如何帮助驯服所有这些高速交换带来的问题。