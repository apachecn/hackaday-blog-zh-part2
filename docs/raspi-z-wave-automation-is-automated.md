# Raspi Z-Wave 自动化是自动化的

> 原文：<https://hackaday.com/2013/10/13/raspi-z-wave-automation-is-automated/>

![raspiAutomationLocksnLights](img/f410dd45e7df6589869540d5b36614c2.png)

家庭自动化在 Hackaday 不断涌现，所以[Cristian Zatonyl]决定与我们分享他的基于树莓 Pi 的系统。这个版本在我们上周进行的[自动化与控制辩论](http://hackaday.com/2013/10/09/ask-hackaday-what-is-home-automation/ "Ask Hackaday: What is “Home Automation”?")的“自动化”方面采取了坚定的立场:不需要用户输入。相反，[克里斯蒂安]依靠[地理围栏](https://en.wikipedia.org/wiki/Geo-fence)来检测他是否已经驶出设定的半径范围，并自动关灯锁门。

这种构建利用了典型的无线遥控设备的 Z-wave 产品，但在 Raspi 上添加了第三方“ [RaZberry](http://razberry.z-wave.me/) 板，使其能够控制现成的 Z-Wave 设备。最后一步是集成一个定制的 iOS 应用程序，该应用程序可以跟踪地理围栏边界，并向 Pi 发出信号来控制灯光和前门的锁。

[Cristian 的]教程涵盖了基础知识，并承认这是一个没有任何安全功能的概念验证。然而，从他的其他 YouTube 视频来看，我们确信更多的开发正在进行中。请观看下面的视频，观看该系统的演示，然后在评论中随意猜测安全问题。我们几年前关于 Z-wave 安全性的文章可能是一个很好的起点。

[https://www.youtube.com/embed/qZyHbGzsfBA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qZyHbGzsfBA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)