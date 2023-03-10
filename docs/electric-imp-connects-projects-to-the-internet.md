# 电动 Imp 将项目连接到互联网

> 原文：<https://hackaday.com/2012/05/17/electric-imp-connects-projects-to-the-internet/>

![](img/6231499849ab4b3fb2120444f418df96.png "imp")

如果你正在计划建造一个与我们一直听说的“物联网”进行无线通信的建筑，你可能想看看[电动 Imp](http://www.electricimp.com/) 。这张小小的卡片将您的项目连接到互联网，而无需配置嵌入式无线设备。

在电动 Imp 内部有一个[好的硬件](http://www.electricimp.com/developers/):一个 ARM CortexM3，和一个 802.11b/g/n wi-fi 模块，它会自动连接到你的无线网络。还有一些引脚用于串行、I2C、SPI 和 PWM 应用。

与手动配置 DNS 和 WPA 加密不同，Electric Imp 会自动完成所有这些工作。~~我们不知道*电动 Imp 如何*配置自己，但我们打赌它是沿着将 SD 卡大小的 Imp 插入计算机并窃取计算机凭证的路线的东西~~。小鬼也使用云服务，但我们敢打赌，一旦小鬼在野外，你将能够在自己的网络中使用它们。

电动 Imp 卡本身的售价约为 25 美元，但也有[开发套件](http://www.electricimp.com/developers/devkits.php)将 Imp 变成 Arduino 兼容板。如果一切按计划进行，小恶魔将在今年夏天的某个时候发布；我们可能会看到一些电动 Imp 项目在 8 月前完成。

编辑:[Kevin]电子 Imp 来信告诉我们配置过程:

> 我们有一个 iOS 和 Android 应用程序，用户输入他们的无线网络的 SSID 和密码，然后他们把屏幕举到 Imp 面前。Imp 中有一个光电传感器，它可以拾取手机的闪光并以光学方式配置设备，而无需将其插入计算机，设置临时网络进行配置，或任何其他繁琐的机制。

我们在这里看到的基本上是一个更酷的版本 [Timex 数据链](http://en.wikipedia.org/wiki/Timex_Datalink)。太棒了。