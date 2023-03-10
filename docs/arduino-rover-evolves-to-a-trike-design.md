# Arduino Rover 演变为三轮车设计

> 原文：<https://hackaday.com/2012/07/05/arduino-rover-evolves-to-a-trike-design/>

![](img/ca955a07dc3cf21ac9cd08f6b0e720b2.png "trike-rover")

[爱德华·罗斯]来信炫耀他的 Arduino 动力自主漫游车的最新版本 ( [翻译](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fwww.entremaqueros.com%2Fbitacoras%2Froshardware%2Farchives%2Fsegundo-robot-autonomo-con-arduino%2F))。你可能还记得在六月份看到的第一个版本。它[从一个遥控卡车车身](http://hackaday.com/2012/06/06/arduino-rover-doubles-up-on-obstacle-avoidance/)开始，增加了一个 Arduino 和一些用于避障的超声波传感器。

两个大轮子和一对传感器看起来很熟悉，但大多数其他组件与该版本不同。最大的变化是从四个轮子过渡到只有三个轮子。这让他放下了控制转向的伺服马达。乍一看，我们认为这东西会弹出一些疯狂的车轮，但实际上行驶的方向拖动第三个轮子是较大的两个。电机本身是不同的，这一次取决于齿轮减速 DC 电机。电机 H 桥是一样的，但[Eduard]使用了一个简单的基于晶体管的反相器，将激活它所需的引脚数量从两个减少到一个。他还从 Arduino Uno 转移到 Nano，以减少控制器的占用空间。