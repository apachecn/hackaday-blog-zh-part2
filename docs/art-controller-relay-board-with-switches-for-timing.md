# 艺术控制器:继电器板，带定时开关

> 原文：<https://hackaday.com/2012/09/13/art-controller-relay-board-with-switches-for-timing/>

![](img/b5c39b9b3a9da0c296b0502cef1b84cf.png "art-controler-relay-with-physical-timing-switches")

[认识艺术控制器](http://www.evilmadscientist.com/2012/artcontroller/)，邪恶疯狂科学家实验室的一款新开发板。它为切换更高电压的负载(但不是电源)提供了一种嵌入式解决方案。我们最喜欢它的一点是无需重新编程固件就能改变开关延迟。

该板使用 ATtiny2313 进行控制。它由板载 7805 线性稳压器提供 5V 稳压电源。该继电器可以处理 24V DC 或 40V 交流负载，其目标受众是需要艺术相关设备的电子开关，但不想每次都设计电路的麻烦。这提供了一个单一的射击，或重复行动，与银行的 DIP 开关选择延迟从每秒一次，每 31 小时。它可以从任何可以拉低引脚的东西获得初始触发，如按钮或硬币接收器。

请记住这一点。项目的开源性质意味着它可以作为参考设计派上用场。