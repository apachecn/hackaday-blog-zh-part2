# 嘿，小植物。让我们做朋友吧！

> 原文：<https://hackaday.com/2014/07/22/hey-there-little-plant-lets-be-friends/>

![poster_01_01](img/da41e240f901b95523cfe3f332b86e63.png)

也许，你的朋友圈子太小了。或者，你只是想和那些扎根在你房子里土壤里的绿叶生物交流。如果是这样的话，这个[环境监测系统](http://hackaday.io/project/1982)将非常适合你！

该项目由[Dickson]创建，可监控室内植物的土壤湿度、空气温度和空气湿度，并在植物缺水时通过电子邮件和短信提醒您。你的豆芽不再会在阳光下枯萎，相反，它们会得到充分的水分，准备好生产它们的蔬菜。

该系统由电池供电，无线，基于 Arduino 和 Raspberry Pi，并配有一个 Android 应用程序，反过来可以让你查看实时和历史数据，从而让你可以选择检查你的叶绿素嵌入式朋友。

[![3116051405904844105](img/494c492cb9aa3e4aa02c638e91db099e.png)](https://hackaday.com/wp-content/uploads/2014/07/3116051405904844105.png)

让我们来看看这个项目中正在使用的传感器。

组成该系统的传感器被安排在一组监控节点序列中。例如，[Dickson]使用一个 Moteino ( [一个带有 RF 收发器](http://lowpowerlab.com/moteino/)的低功率 Arduino 克隆)、一个土壤湿度传感器、一个湿度传感器、一个温度传感器和一个电池表。主传感器节点收集数据，并通过收发器在 915mhz ISM 频段上将其传输到基站。从那里，基站容纳另一个 Moteino，它充当接收 RF 信号的网关，以及一个 Raspberry Pi，其中数据存储在 MySQL 数据库中，并将信息馈送到 Plant Friends 移动应用程序。

[Dickson]该项目的目标是将其发布到全世界，以便其他初学者也可以学习如何开发类似的工厂监控系统。

让这个想法更好的是，所有的组件都可以放在可爱的定制竹盒中，让你感觉你的朋友群变得更大了。

[![poster_04_01](img/10f590c9d41e2c83cb95fbf5091e930f.png)](https://hackaday.com/wp-content/uploads/2014/07/poster_04_01.jpg) 想了解更多关于这个项目的信息和看到更多可爱的照片，一定要在[【迪克森】的主页上查看](http://dicksonchow.com/plantfriends)的操作指南。完整的说明也可以在上面的第一个链接中找到。

另一个值得一试的黑客技术是这个[雨水桶灌溉系统，当你太忙的时候，它可以为你的室外植物提供养分](http://hackaday.com/2012/03/29/rain-barrel-irrigation-system-keeps-your-plants-fed-when-youre-too-busy/)，我们在 2012 年报道过这个系统。