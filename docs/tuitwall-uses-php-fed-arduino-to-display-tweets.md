# Tuitwall 使用 PHP 支持的 Arduino 来显示推文

> 原文：<https://hackaday.com/2012/09/18/tuitwall-uses-php-fed-arduino-to-display-tweets/>

![](img/af035d087c0853f84e08795cc61af629.png "tuitwall-hardware")

[圣地亚哥]最近完成了这个项目，他称之为 Tuitwall。它会在 LED 矩阵上显示你的推特信息。他用来组合的方法对于任何需要从互联网上搜集信息的项目来说都会很方便。

除了上面看到的 Arduino 硬件，该项目还需要一台服务器。在 Arduino 方面，[Santiago]使用以太网屏蔽和 LED 矩阵，通过 SPI 寻址。服务器正在运行一个 PHP 脚本，该脚本利用 twitteroauth 库来处理认证。

需要做一点点配置，大部分都与 Twitter 如何处理第三方应用程序有关。但是一旦一切都设置好了，你就可以随身携带硬件，并将其接入任何网络(只要它提供 DHCP)。有了这个框架作为指导，按照你的意愿改变它是轻而易举的事。它可以用作 RSS 阅读器、时间和温度、服务器群状态、显示假标题的恶作剧票等。