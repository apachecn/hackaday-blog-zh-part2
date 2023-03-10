# 黑客日奖品入口:Arduino MPPT 控制器

> 原文：<https://hackaday.com/2015/05/23/hackaday-prize-entry-arduino-mppt-controller/>

想象你正在建造一个小型太阳能装置。天真的解决方案是从恐怖货运公司拿一块太阳能电池板，一个汽车电池和交流逆变器，然后希望一切正常。这是愚蠢的解决方案。为了充分利用太阳能，你需要使太阳能电池的电压与电池的电压相匹配。你是怎么做到的？随着[Debasish]获得 Hackaday 奖，一个 Arduino MPPT 太阳能充电控制器。

这个[最大功率点跟踪器](http://www.instructables.com/id/ARDUINO-SOLAR-CHARGE-CONTROLLER-Version-30/step2/Basics-on-MPPT-charge-controller/)使用降压转换器将太阳能电池的电压降低到电池的电压。它的效率极高，每一个合适的太阳能装置都需要一个充电控制器来做类似的事情。

对于他的 MPPT，[Debasish]正在使用一个 Arduino Nano 进行所有的计算，一个 DC 到 DC 降压转换器和几个 MOSFETs。非常简单，但是[Debasish]是用一个 ESP8266 模块将整个控制器连接到互联网。这是一个很好的例子，用比买同样的东西低得多的成本来制造东西，也是一个很好的例子，说明有机会让世界变得更好的东西。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)