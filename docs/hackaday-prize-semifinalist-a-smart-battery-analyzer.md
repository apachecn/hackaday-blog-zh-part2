# Hackaday 奖半决赛选手:智能电池分析仪

> 原文：<https://hackaday.com/2015/08/30/hackaday-prize-semifinalist-a-smart-battery-analyzer/>

[K.C. Lee]参选黑客日奖不会治愈癌症，从地球上消除疾病，阻止外星人入侵，或拯救世界。[他的电池充电器和分析器](https://hackaday.io/project/4993-dual-channel-battery-chargeranalyzer)是一个有用的小装置，用于确定电池的充电和放电特性，也可以用作双通道电子负载、电流源或电源。

在[K.C.]的设备中有锂离子电池、铅酸电池和镍氢电池充放电所需的所有工具。他用一些稍微不寻常的电路做到了这一点，包括一个 [SEPIC DC 到 DC](https://en.wikipedia.org/wiki/Single-ended_primary-inductor_converter) 转换器，和一个“模拟”PWM 控制器。这两种技术共同意味着[K.C.]可以在设计中使用更小的电容和电感，这也意味着输出端的纹波更小。至于电池充电器和放电去，这是一个非常好的设计。

电池放电和充电的控制通过带 USB 的基于 SILabs 8051 的微控制器进行。用户界面是一个简单的诺基亚液晶显示器和一个运行在 Windows 中的应用程序。如果你想拯救世界，这个项目不适合你。如果你需要测试一些充电电池，这是一个很好的设备。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)