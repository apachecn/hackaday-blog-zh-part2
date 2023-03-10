# 钻研 ARM 编程的最简单方法

> 原文：<https://hackaday.com/2012/09/09/the-easiest-way-to-dive-in-to-arm-programming/>

[Brad]对恩智浦发布的 ARM Cortex-M0 芯片感到非常兴奋；这是一个功能齐全的 ARM 微控制器，非常令人惊讶的是，它被塞进了一个爱好者和试验板友好的 DIP-28 封装中。在找到该芯片的供应商后，[Brad]投身其中，用开源工具编写了一个很棒的教程，用于[在试验板上对手臂进行编程。](http://www.meatandnetworking.com/tutorials/lpc1114fn28-with-open-source-tools/)

问题中的芯片是恩智浦的 [LPC1114FN28](http://www.nxp.com/products/microcontrollers/cortex_m0/lpc1100_x_l/LPC1114FN28.html) ，这是一款 28 引脚试验板友好芯片[，我们之前已经发布过。](http://hackaday.com/2012/08/13/the-coming-age-of-arm-chips-for-the-hobbyist/)找到[这款微控制器的单一供应商](http://avnetexpress.avnet.com/store/em/EMController/Microcontroller/NXP-Semiconductors/LPC1114FN28-102-12/_/R-5003286402656/A-5003286402656/An-0?action=part&catalogId=500201&langId=-1&storeId=500201&listIndex=-1&page=1&rank=1)(一个芯片只要 1.26 美元！)，[布拉德]拿出他的试验板，开始接线。

因为这个微控制器有一个板载振荡器，所以连接试验板和为 FTDI 电缆安装一个分线点很容易。在[配置工具链](http://www.meatandnetworking.com/tutorials/arm-cortex-mx-quickstart/)并编写一点代码之后，唯一的问题是将代码上传到芯片。这是由 [lpc21isp](http://sourceforge.net/projects/lpc21isp/) 编程工具处理的，由【布拉德】稍微修改和配置，以支持他最喜欢的微控制器。

LPC1114FN28 是一个令人印象深刻的套件，有了免费的工具来编程这该死的东西，我们不能等待自制的 ARM 开发板出现。