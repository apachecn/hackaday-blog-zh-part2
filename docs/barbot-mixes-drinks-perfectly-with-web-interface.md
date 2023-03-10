# Barbot 通过网络界面完美混合饮料

> 原文：<https://hackaday.com/2013/12/31/barbot-mixes-drinks-perfectly-with-web-interface/>

![barbot-with-laptop](img/b8d71ac6fa703993bba5d3c772e31597.png)

你擅长调饮料吗？我们认为这个机器人可能会让你大赚一笔！

这款酒吧机器人不仅可以容纳 5 种不同的酒，而且你可以用[一个非常光滑的网络界面将它们任意组合，你可以自己查看](http://barbot.seancarney.ca/)。

在初始设置期间，您将选择的液体添加到机器中，然后使用网络界面中的[配置模式](http://barbot.seancarney.ca/config)，您告诉 Barbot 它必须使用什么。一旦这些字段被填充，Barbot 将列出它能够与所提供的成分混合的各种饮料。它还有一个清洁模式，允许你启动泵，并为你的聚会设置管理权限。

这一构建背后的硬件是 BeagleBone Black，运行 Ubuntu 13.04，使用 Apache2、MySQL 和 PHP 来托管 web 界面——bind 和 DHCP 用于使用 USB WiFi 加密狗创建 web 门户。在线界面通过 GPIOs 使用 PHP 直接控制泵。

休息后观看完整的演示视频。

[https://embedr.flickr.com/photos/11443998346](https://embedr.flickr.com/photos/11443998346)