# 另一个出奇相似的高功率 LED 驱动器黑客

> 原文：<https://hackaday.com/2012/09/20/another-eerily-similar-high-power-led-driver-hack/>

![](img/c8d1baaf581260ddcdf9a94319a35b21.png "HighPowerLEDFader")

[Maximilian Güntner]在上周的全球报道中给我们留下了一条评论，链接到他自己的项目，其中涉及一个类似的高功率 LED 驱动器模块。这看起来和我们想出的一模一样，[Güntner]甚至用这种模式将一束高功率 LED 连接到 PCA9685 LED 驱动器[ [pdf](http://www.nxp.com/documents/data_sheet/PCA9685.pdf) ]。这和[迪斯科星球](http://hackaday.com/2012/09/11/disco-planet-a-massive-rgbw-led-array-in-a-6-globe/ "I really did come up with it all on my own, this is insane!")的概念一模一样！

人们用这种方式改造大功率 led 驱动器已经有一段时间了，这不足为奇。每把只有几块钱，输入电压范围很大。在[Güntner]的案例中，他从 Dealextreme 那里抓了一堆这些。实际上，网站上还有两个[和其他](http://www.dealextreme.com/p/mr16-1-3w-650-700ma-constant-current-regulated-led-driver-8-40v-input-13557)，这三个网站都有评论(可以追溯到一年前),提供各种修改小 PCB 的有用提示。

我们的易趣来源的董事会是不同的。[Güntner]购买的电路板采用 PowTech PT4115 [ [pdf](http://www.micro-bridge.com/data/CRpowtech/PT4115E.pdf) ，它使用的器件更少，数据手册也更容易理解。举个例子，旁边有一个小小的脉冲宽度调制信号的管脚优雅地标上了“DIM”。神经！易趣的司机使用 MCP34063 [ [pdf](http://www.onsemi.com/pub_link/Collateral/MC34063A-D.PDF) ]，它有一个更神秘的数据表(烧了两周和几个笔记本页面来找出电路)。最终，这两者是如此的相似以至于没有区别。

因此，如果你想自己修改一些 LED 驱动程序，可以在跳转之后查看操作视频。谢谢！

[https://www.youtube.com/embed/sohPA29wnFo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sohPA29wnFo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)