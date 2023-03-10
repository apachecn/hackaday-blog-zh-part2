# Hackaday 奖参赛作品:FPGA 驱动的推进器

> 原文：<https://hackaday.com/2015/07/21/hackaday-prize-entry-an-fpgad-propeller/>

视差推进器是一个格外有趣的芯片，却没有得到应有的爱。它是一个 32 位微控制器，有八个独立的内核，每个内核都足够强大，可以进行一些真正的计算。大约在去年的这个时候，[Propeller 的源代码被开放](http://hackaday.com/2014/08/07/parallax-propeller-1-goes-open-source/)并在 GPL 3.0 下发布，同时发布的还有 mask ROM 和 Propeller 专用语言 Spin 的解释器。这次发布不仅是一个很好的教育机会，也是一个极好的机会来建造一些真正酷的硬件，就像[正在用软螺旋桨](https://hackaday.io/project/6786-soft-propeller)做的那样。

[antti]的软推进器基于 [Xilinx ZYNQ-7000](http://www.xilinx.com/products/silicon-devices/soc/zynq-7000.html) ，这是一个片上系统，它将双核 ARM Cortex A9 与具有足够逻辑门的 FPGA 相结合，成为一个推进器。该板还具有 16MB 的闪存用于配置，一切都适合与螺旋桨兼容的 DIP 40 引脚排列。如果你曾经想玩 FPGAs 和高功率 ARM 设备，这是你的项目。

[antti] [已经在他的板](https://hackaday.io/project/6786-soft-propeller/log/21165-sd-test-prop-code)上运行了 Propeller Verilog，并且使用了略多于 50%的 lut，它甚至有可能将即将到来的 Propeller 2 安装在这个芯片上。这个构建只是一个更大更雄心勃勃的项目的一小部分:[antti] [正在开发一个类似的设备](https://hackaday.io/project/6826-soft-propeller-hdmi-usb)，带有 HDMI、USB、MicroSD 和 32MB DDR2 RAM。这也将被填充到 DIP40 格式中，使其成为一个功能强大得令人难以置信的系统，仅比一根口香糖大一点点。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)