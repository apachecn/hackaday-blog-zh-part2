# (蓝色)组合中的另一个物联网平台

> 原文：<https://hackaday.com/2015/07/23/another-iot-platform-in-the-bluemix/>

许多大公司(例如，英特尔、甲骨文、Atmel 和 IBM)都在竞争成为物联网的标准互连结构。作为一名开发人员，很难通过市场宣传来判断哪个平台最适合您和您的应用程序。幸运的是，网上有大量展示这些框架的项目。这些项目网站是一种评估物联网框架在实际应用中的优缺点的简单方法，而不必自己开发原型。

例如，[diyhacking]发布了一个使用 IBM 的 Bluemix 和一个 Raspberry Pi 来完成一些简单的家庭自动化任务的演示。该项目硬件适中，使用 PIR 运动传感器和继电器来控制交流负载。然而，这很好，因为它让您专注于 Bluemix 工具。示例客户端和服务器软件不到 [200 行的 Python](https://github.com/DIYhacking/IoT) 。

Bluemix 看起来与 Raspberry Pi 有很好的集成，并且有一个模拟器，所以你可以在没有真正的硬件开发的情况下工作。Bluemix 确实提供免费计划([有限制](https://console.ng.bluemix.net/pricing/))，但收费选项可能会让一些物联网黑客望而却步。

[https://www.youtube.com/embed/8xS8cP-PWM8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8xS8cP-PWM8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

然而，令人惊讶的是，看到一个家庭自动化继电器(据推测，是携带墙电流)放在一个无焊试验板上。虽然这在理论上没有错，但在实践中往往是个坏主意。

这仍然不会阻止你将这个项目与 [Thingspeak](http://hackaday.com/2015/07/19/the-internet-of-soldering-irons/) 或其他[平台](http://postscapes.com/internet-of-things-platforms)进行比较。