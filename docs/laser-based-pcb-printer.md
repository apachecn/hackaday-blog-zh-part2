# 基于激光的 PCB 打印机

> 原文：<https://hackaday.com/2014/02/03/laser-based-pcb-printer/>

能够在家里制作 PCB 是 DIYer 武库中的一个里程碑。无论你是用物理方法还是化学方法蚀刻电路板，要做到完美都是一项棘手的任务。[Charlie & Victor]正在努力解决这个复杂的杂务。他们称他们的机器为 DiyouPCB。DiyouPCB 是一个开源的 PCB 蚀刻项目，由硬件和软件组件组成。

该项目是基于使用蓝光光学拾波器。该拾取被完整地使用，没有任何修改，以简化构建过程。为了使用拾音器，[Charlie & Victor]必须对通信协议进行逆向工程，这也允许他们利用读取蓝光光盘时使用的自动对焦功能。这台机器的框架让人想起 RepRap，他们用它来做初步测试和激光调谐。X 轴和 Y 轴在黄铜轴衬上运行，由步进电机驱动，步进电机由 Arduino 通过专门设计的 DiyouPCB 控制器护罩控制。

为了开始该过程，将空白 PCB 板切割成最终的板尺寸。在将纸板正面朝下放在机器上之前，将光致抗蚀剂干膜涂在纸板的一面。使用 [Cadsoft Eagle](http://www.cadsoftusa.com/eagle-pcb-design-software/?language=en) PCB 设计软件生成 PCB 设计，并导出为 HPGL 文件。DiyouPCBRun 软件将 HPGL 信息发送到自定义编写的 Arduino 固件，该固件进而使用 DiyouPCB 控制器屏蔽控制步进电机和光学拾取器。光学拾波器的激光从电路板的无痕区域去除光刻胶膜。然后通过酸浴蚀刻掉暴露的铜，接着剥离剩余的光致抗蚀剂膜以暴露铜迹线。结果是一个完整的 PCB 板。

诚然，PCB 结果并不完美。步进电机被认为是导致振动的原因，这可以在一些蚀刻画中看到。轴加强和车架阻尼降低了振动，但没有消除振动。为了进一步解决振动问题，[Charlie & Victor]正在讨论升级到伺服电机，或者通过用丝杠代替皮带来牺牲速度。

如果你想知道如何得到一台这样的机器，这很简单。[Charlie & Victor]已经在他们的网站上提供了所有必要的[项目文件](http://www.diyouware.com/download)供您下载，包括 3D-printable。stl 文件、软件和控制器屏蔽。

[https://www.youtube.com/embed/x9WxdGmGvyY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/x9WxdGmGvyY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)