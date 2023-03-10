# JTAGulator 查找调试接口

> 原文：<https://hackaday.com/2013/10/02/jtagulator-finds-debug-interfaces/>

![jtagulator](img/02511aea7c20747c5a61a79289817415.png)

[Joe Grand]提出了一个工具，我们认为它对任何试图入侵物理设备的人都有用:JTAGulator。在我们的 DEF CON 报道中，我们[简单地提到了 JTAGulator](http://hackaday.com/2013/08/04/def-con-tamper-evidence-contests-and-embedded-talks/) ，但是它确实值得一个更深入的特性。JTAGulator 是一种在不熟悉的硬件上发现片上调试(OCD)接口的方法。

今天，打开任何手机、路由器或任何中等复杂的设备，你都会找到测试点。通常，这些测试点中至少有几个是通用的 JTAG / IEEE 1149.1 接口。

JTAG 接口有 5 个基本引脚:TDI(测试数据输入)、TDO(测试数据输出)、TCK(测试时钟)和 TMS(测试模式选择)、/TRST(测试复位)(可选)。

如果你在看一个有很多测试点的 PCB，哪些是 JTAG 引脚？还有哪些测试点是哪些信号？有时候 PCB 厂商会在丝印上给出线索。其他时候你都是一个人。[Joe]设计了 JTAGulator 来帮助找到这些引脚。

想法很简单:将 JTAGulator 连接到被测 PCB 上的测试点，通过串行终端发出几个命令，让 JTAGulator 完成剩下的工作。它对引脚的每一种排列执行强力方法，发出基本的 JTAG 命令 IDCODE 或 BYPASS，并寻找响应。如果收到任何有效的响应，JTAGulator 将显示找到的接口的引脚。

[乔]使用视差推进器作为他设计的核心。他增加了输入保护、可选电压(1.2V 至 3.3V)和总线盗版兼容接头。JTAGulator 还可以识别和测试串行 UART 引脚，以确定是否存在任何串行端口。如果 JTAG 和串行还不够的话，JTAGulator 是完全开源的，在 3.0 美国许可证下发布。您可以添加任何想要的接口。尽管[Joe]计划在未来增加更多的通用接口。

[https://www.youtube.com/embed/uVIsbXzQOIU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uVIsbXzQOIU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)