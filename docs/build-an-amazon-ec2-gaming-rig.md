# 建立一个亚马逊 EC2 游戏平台

> 原文：<https://hackaday.com/2015/07/10/build-an-amazon-ec2-gaming-rig/>

电脑游戏比游戏机游戏更好。既然我们已经说了一些足以满足这篇文章评论配额的有争议的事情，让我们深入研究一下[【拉里】的亚马逊 EC2 游戏装备](http://lg.io/2015/07/05/revised-and-much-faster-run-your-own-highend-cloud-gaming-service-on-ec2.html)。

前阵子，[拉里]买了一台 MacBook Air。就其本身而言，这是一台很棒的机器，但它并不是你想要在旅途中玩现代 AAA 游戏的笔记本电脑。如果您有足够的带宽和足够低的 ping，那么您几乎可以复制 EC2 实例的所有内容。

[Larry]在他的实例中使用的是带有单个 NVIDIA GRID K520 GPU 的 Windows Server 2012 AMI。在配置好所有的安全、防火墙和其他基本东西之后，只需要为 NVIDIA Titan 安装一个特定的驱动程序。安装了 Steam 并正确配置了家庭流媒体后，就可以开始游戏了。

拉里在这种环境下的表现令人印象深刻。这是 60fps，但因为他将所有的游戏都传输到 MacBook Air，他永远不会得到 1080p。

如果你想知道这要花多少钱，[它实际上并不太糟糕](http://lg.io/2015/04/12/run-your-own-high-end-cloud-gaming-service-on-ec2.html)。拉里基于云的游戏系统的第一个版本大约是每小时 0.54 美元。对于 1000 美元的战斗工作站来说，这相当于 1900 小时的游戏时间，而对于 400 美元的土豆来说，这相当于 740 小时的游戏时间。