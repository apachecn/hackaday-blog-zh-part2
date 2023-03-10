# 使用开源工具的 STM32 F4 探索教程

> 原文：<https://hackaday.com/2012/09/27/stm32-f4-discovery-tutorial-using-open-source-tools/>

![](img/1a50ead70e441bd1941117f0bdd393fc.png "STM32F3_discovery_kit_p3323big")

[Pulko Mandy]拿到了新的 STM32 F3 发现板。他和我们一样是开源工具的粉丝，所以他发布了一个指南，介绍了如何在 F3 硬件上使用开源工具链。

这个板在本月早些时候刚刚发布，但是在 OpenOCD 中已经有了对它的支持。这与 F4 董事会没什么不同，我们会认为它让这个过程变得简单了一些。[Pulko]正在使用 Sourcery CodeBench Lite 工具链，它适用于几乎所有的 ARM 芯片。它是基于 GCC 的，并附带了用于调试的 GDB(以及您期望的所有其他工具)。他确实创建了自己的链接器脚本和启动代码。这些对 ARM 来说至关重要，所以他能为我们提供这些东西真是太好了。他在指南的最后展示了如何使用 OpenOCD 将代码刷新到芯片上，以及它如何与调试器一起工作。

[ [照片来源](http://www.st.com/internet/com/press_release/p3323.jsp)