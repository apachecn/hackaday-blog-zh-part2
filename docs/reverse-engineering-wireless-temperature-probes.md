# 逆向工程无线温度探头

> 原文：<https://hackaday.com/2015/03/01/reverse-engineering-wireless-temperature-probes/>

住在落基山脉的正对面，有一段时间他想测量他的房子内部的温度变化和外面的温度波动。明智的做法是在房子周围放置几个无线温度记录探头，并用电脑记录所有数据。一个温度传感器、微控制器、无线模块、电池、外壳和各种零件意味着传感器网格中的每个节点将花费大约 10 美元。前几天，[bhunting]在沃尔玛的清仓里遇到了完全一样的东西——10 美元一个无线温度传感器，[，他唯一要做的就是逆向工程协议](http://www.techspin.info/archives/985)。

这些无线温度传感器正是你在沃尔玛清仓中发现的廉价中国电子产品。在一滴环氧树脂下有一个工作在 433MHz 的小型无线电，一个温度传感器和一个微控制器。温度传感器中的微控制器和发射器板仅通过带状电缆连接，每条线路都贴有标签。在找到电源和接地后，[bhunting]用示波器检查了向无线电[提供数据的电线，并用逻辑分析仪](http://www.techspin.info/archives/1049)对其进行了检查。

经过一番努力，【bhunting】能够弄清楚温度传感器是如何将数据发送回基站的，[并对其中一个基站](http://www.techspin.info/archives/1056)做了一点手术，他有办法用 Arduino 读取温度数据。从那以后，这只是一个数据记录问题，用 Excel 很容易解决，而[bhunting]正是他最初想要的，这要感谢沃尔玛清仓箱中的一个发现。