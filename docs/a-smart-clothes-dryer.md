# 智能干衣机

> 原文：<https://hackaday.com/2014/05/28/a-smart-clothes-dryer/>

![dryer6](img/2672cc6c9f2a775899cc983db573daee.png)这里有个问题会让你绞尽脑汁:衣服干了你的干衣机会停吗？似乎如果你有一台机器，它为了一个单一的目的而消耗能量，你会希望它在工作完成后停下来，或者为了方便起见，继续运转直到衣服干了。温度和湿度传感器很便宜，如果你没有自动感应干衣机，[一个 DIY 智能干衣机](http://www.thebmwz3.co.uk/article.php?story=20140527140011464)看起来既高效又方便。【来自未来的编辑:林克腐，[好像现在就在这里](http://www.thebmwz3.co.uk/2014/05/clothes-dryer-arduino-moisture-alert.html)。]

我想当衣服干了，它们就不会散发湿气了。基于这一前提，他可以监控干衣机的运行，或者关闭机器，或者发送一条信息，该把衣服拿出来了。这是一个非常简单的想法，有了 Arduino 和 DHT11 温度和湿度传感器，组装起来相当容易。

用于本实验的干衣机是一种不通风的自通风型干衣机。相反，它会将毛巾和牛仔裤中的水冷凝到一个桶中，稍后用手清空。这可能会在测试中引入一点误差，但[安迪]确实想出了一种方法来安装温度传感器，而不用以任何方式修改他的烘干机。从最初的数据来看，无通风口烘干机可能会引入一点实验误差，但这仍然是一个很好的想法，不要用传统的向外通风的烘干机来尝试。如果你想亲自尝试，这是代码。