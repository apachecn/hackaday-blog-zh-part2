# 状态灯告诉你密码又被破解了

> 原文：<https://hackaday.com/2013/12/12/status-light-tells-you-the-code-is-borked-again/>

![status light](img/249a7cf40d619b2f7043c2d13fe2f870.png)

[亚瑟]正在自学产品开发。他没有创造一些模型产品，而是走上了设计他可以使用的真实设备的道路。他目前的设备是自动化软件测试的状态灯。我们之前已经见过[测试](http://hackaday.com/2012/02/12/monitoring-software-builds-with-a-traffic-light/)和 [GitHub](http://hackaday.com/2013/10/16/monitor-github-activity-with-an-rgb-led-matrix/) 状态灯，然而这是第一个与外部网络服务集成的。状态灯的状态基于在线持续部署测试引擎 [CodeShip](https://www.codeship.io/) 的输出。

电子设计很简单。电子 Imp 从 CodeShip 检索测试状态数据。然后，Imp 通过两条 GPIO 线将状态数据发送到 AdaFruit 饰品。饰品控制一个新像素的戒指。绿色环表示所有测试都通过。紫色表示测试正在进行中。旋转的红色环(死亡)意味着一个或多个测试失败。通过迷你 USB 连接器供电。

[Arthur]在状态灯的机械设计上也花了不少时间。所有零件都是 3D 打印的。这使得他可以快速地对每个部分进行多次修改。我们喜欢在灯的顶部使用白色 PLA 作为磨砂效果，因为它扩散了所有 RGB LEDs 发出的刺眼光芒。作为点睛之笔，[Arthur]为他的 light 制作了一个假的[产品页面](https://arthurguy.co.uk/portfolio/status-light)。他没有任何出售它的计划，但我们希望他放弃源文件和 STL 文件，这样我们就可以创建一个我们自己的。

[https://www.youtube.com/embed/qJZfI9asG-8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qJZfI9asG-8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)