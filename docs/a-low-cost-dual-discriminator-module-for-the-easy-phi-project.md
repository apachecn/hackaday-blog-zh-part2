# Easy-phi 项目的低成本双鉴别器模块

> 原文：<https://hackaday.com/2014/01/03/a-low-cost-dual-discriminator-module-for-the-easy-phi-project/>

[![](img/a47c212b6e32b1ade2a257a113a34faf.png)](http://hackaday.com/wp-content/uploads/2014/01/univ_input_angle.jpg)

几个月前，我向您展示了 Easy-phi 项目，该项目旨在为业余爱好者构建一个简单、廉价但智能的基于机架的开放硬件/软件平台。有了 easy-phi，您只需在一个机架上添加卡(如上图所示),即可实现您想要的功能。

最近，我的团队完成了对我们基于 FPGA 的鉴别器(如果你喜欢的话，也可以称为“通用输入”)的测试。由于 easy-phi 卡使用明确定义的电信号相互通信，我们需要制作一种能够翻译来自外部的不同类型的电信号并执行大量其他功能的卡。因此，它被设计为具有 100MHz 输入带宽，带有交流/DC 耦合 50 欧姆/高阻抗输入级(x2)和 4 个 easy-phi 输出。对于该模块，我们选择了(旧的)spartan3-an FPGA 来执行最终用户可能需要的不同逻辑功能(高速计数器、OR/XOR/AND、脉冲创建等)。利用板上的 cortex-m3 微控制器，可以轻松地随意重新配置。所有的设计资源都可以在我们的 [Github](https://github.com/easy-phi/main) 上找到，你也可以随时看看我们的[官网](http://www.easy-phi.ch/)。