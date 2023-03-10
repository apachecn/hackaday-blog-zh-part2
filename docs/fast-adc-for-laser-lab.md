# 快速 ADC 使用 48 MSPS 的老学校范围黑客

> 原文：<https://hackaday.com/2015/07/21/fast-adc-for-laser-lab/>

[Carlos]他的激光实验室需要一个采样周期为 50 纳秒的 ADC，即 20Msps！(每秒 2000 万个样本)。虽然近年来，已经有了达到低 GSPS 的商用 ADC，但集成采集系统仍然有些昂贵。所以[卡洛斯]决定像每个优秀的黑客一样，建立自己的解决方案。[他的项目帖子](https://hackaday.io/project/6836-adc-speed-upgrade)几乎只是链接到[他写的一份白皮书](https://www.dropbox.com/s/ze40em4vbre0gzb/writeup.pdf?dl=0) (PDF)，所以我们试着为你总结一下:

为了简化开发[Carlos]借用了第一个数字示波器时代常用的技术，等效采样时间。

[![est](img/fcd73897454316188cb9bdcaeccceed3.png)](https://hackaday.com/wp-content/uploads/2015/07/est.png)

右图来自[TDS 460](http://www.trs-rentelco.com/Manual/TEK_TDS420A_Manual.pdf)T2 手册。虽然对于那些只熟悉现代示波器的人来说，这似乎有悖直觉，但 TDS460 使用 100MSPS ADC 实现了 400MHz 带宽。为了实现这一点，示波器在多个周期中采集单个轨迹，每次如图所示偏移采集并组合结果。

这样，早期的数字示波器开发人员就可以避开现有 ADC 的限制，获得更高的有效带宽。然而，当然有一个问题:该技术仅适用于周期信号。

这对[Carlos]来说很好，他在[Cypress PSoC 4](http://hackaday.com/2014/06/16/cypress-launches-5-arm-dev-board/)上实现了一项技术，提供了类似模拟 FPGA 的功能。通过偏移 ADC 触发器，他能够使用 1MHz 的 ADC 采样实现 48MHz 的 EST。如果你想得到一点帮助自己进入 PSOC 4，看看【比尔·赫德】制作的指南[。](http://hackaday.com/2014/04/23/getting-your-feet-wet-with-programmable-system-on-chip/)

我们希望将来能听到更多关于你的激光实验室的消息。