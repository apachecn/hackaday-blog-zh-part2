# 用软件无线电探测银河自转

> 原文：<https://hackaday.com/2013/05/26/detecting-galactic-rotation-with-software-defined-radio/>

去年夏天，在通过 USB 电视调谐器的软件定义无线电的全盛时期，我们向 hackaday 的读者提出了一个问题:[有人在使用大家最喜欢的 SDR 方法进行射电天文学吗？](http://hackaday.com/2012/06/17/ask-hackaday-has-anyone-built-a-radio-telescope/)花了将近一年的时间，终于有了一个将 USB 电视调谐器变成射电望远镜的了不起的项目。[它来自【马库斯·利奇】](http://www.sbrac.org/files/budget_radio_telescope.pdf) (PDF 警告)的丰富思想，足以用一个三英尺的卫星天线探测到银河系的旋转。

RTL-SDR.com 的[卡尔]为我们带来了[马库斯]工作的消息，他一直在密切关注在后院建造射电望远镜的进展。他已经收集了许多有趣的珍闻，包括[这张 gif](http://www.sbrac.org/files/gp-+59-anmiated.gif) 图，显示了在几个小时的过程中，一个星系臂进入和离开【马库斯】望远镜的视野。

[马库斯]的望远镜不仅可以记录 continium 的测量结果——基本上，一个单像素相机只对一个频率敏感——它还可以产生天空的光谱图。将同时测量多个频率的能力与多普勒效应结合起来，[马库斯]可以用 USB 电视调谐器测量星系的旋转。这在我们看来太棒了。

如果你已经有一个 RTL-SDR 电视调谐器和一个较大的卫星天线，[马库斯]的项目应该是相当便宜的复制；馈送组件由一个咖啡罐制成，放大器是重新利用的卫星电视设备，所有的软件——[ Marcus]自己的 GNU Radio 工具——都是开源的。当然，用一个 3 英尺直径的碟形天线，复制大型射电望远镜的数据是不可能的。尽管如此，这仍然是一件令人印象深刻的工作，让我们在 craigslist 上搜索旧的 C 波段菜肴。