# Easy-phi:面向实验者的开源平台

> 原文：<https://hackaday.com/2013/10/22/easy-phi-an-open-source-platform-for-experimenters/>

[![](img/c490eb098b934d3568cfdbabb578d05f.png)](http://hackaday.com/wp-content/uploads/2013/10/rack_28f_inside.png)

一些 Hackaday 的读者可能已经知道，我的日常工作包括与高速电子设备打交道。在过去的几个月里，我在瑞士日内瓦大学的团队一直致力于一个面向实验者的开源平台:easy-phi 项目。主要想法是建立一个简单、便宜但智能的开放硬件/软件平台，由 19″框架(或更小)组成，可以容纳各种各样的电子模块。因此，业余爱好者只会制造/购买适合他们需求的模块，并通过网页/独立应用程序/ Labview 模块来控制它们。

我在我的网站上详细介绍了这个项目的技术方面。为了给你一个快速简单的概述，[机架](http://www.limpkin.fr/index.php?post/2013/09/98/Easy-phi-project%3A-the-rack-and-its-backplane)本质上是一个 USB 集线器，它将所有模块连接到一个 Cubieboard。它还集成了一些同步信号、时钟和电压、温度、功耗监控系统。[模块](http://www.limpkin.fr/index.php?post/2013/10/09/Easy-phi-project%3A-the-template-module)由模板+模块专用电子设备组成。模板电子设备是“easy-phi 标准”的一部分，它们由 Arduino 兼容的 SAM3X8E 微控制器和一些其他与电源相关的组件组成。这确保了你们可能开发的机架和模块之间的电气和固件兼容性。值得注意的是，模块在 USB 总线上被列举为复合 CDC(通信设备)和 MSC(大容量存储器)。CDC 用于配置模块，而 MSC 允许您获取其文档、资源和独立应用程序，以防您在没有机架的情况下使用模块。

选择的原理图/布局软件是 Kicad，所有当前文件都可以在我们的 [github](https://github.com/easy-phi/main) 上找到。一旦我们测试了当前管道中的其他模块，其他模块将被上传。由于我们正在开发的是面向物理的，我们希望爱好者将 easy-phi 带到其他领域。如果您有任何问题或者您想做出贡献，请不要犹豫与我们联系。