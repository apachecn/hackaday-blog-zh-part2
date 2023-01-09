# STM32 驱动 PCIe 显卡

> 原文：<https://hackaday.com/2012/10/08/stm32-driving-a-pcie-video-card/>

![](img/99c9fe9c9a824902826692393ed31a0f.png "mst32-driving-a-pcie-video-card")

[Gpuhackr]选择他的用户名来准确地解释他如何度过他的时间。例如，这里他正在使用 STM32 发现板驱动 AMD 镭龙 HD 2400 显卡。ARM 微控制器实际上并没有使用卡上的 PCIe 接口。相反，[Gpuhackr]已经修补到卡本身内置的调试接口中。这并不像听起来那么简单，但如果你仔细布线，这是一种非常有趣的连接手臂和液晶显示器的方式。

如果不是 AMD 发布的开源代码，这个项目几乎是不可能的。这让他可以实现该卡的 3D 渲染功能。该演示直接对视频卡上的 UVD Xtensa CPU 进行编程。它绘制了一个每边都有颜色渐变的立方体。当调试信息覆盖在屏幕上时，立方体旋转。在这种情况下，ARM 芯片/板实际上被用作程序员来上传一些定制固件。但是我们认为一个真正的代码忍者可以实现一个通信协议来打开一个实时驱动卡的简单方法。

[感谢提示]