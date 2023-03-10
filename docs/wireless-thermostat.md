# 无线恒温器

> 原文：<https://hackaday.com/2014/01/05/wireless-thermostat/>

![thermostat0104](img/e0764bfd758d56e8fb33f8d86863cc23.png)

在[汤姆] 100 年历史的房子里，恒温器离炉子的位置有两层楼高，所以墙上一根断了的电线正是设计无线恒温器所需的催化剂。

这个系统是基于一个定制的 PCB [Tom]设计的，叫做[魔法微粒](http://smokedprojects.blogspot.com/2013/12/magicmote-wireless-sensor-node.html)。该板包含一个 MSP430 微控制器、一个低功耗 NRF24l01+无线收发器和各种传感器接口。无线恒温器项目使用两块这样的板；一个监控二楼的温度，一个控制地下室的炉子。

温度检测利用 DHT22/AM2303 温度和湿度传感器完成，这是一个方便的选择，因为该器件经过校准并处理模数转换；您只需要一个数字引脚来检索温度/湿度数据。为了控制熔炉，[Tom]使用本地 24v 交流电和一个闭锁继电器来驱动加热器信号。24 伏交流电也给电路板供电，所以门铃变压器把电压降低到更有用的水平；大约 11VAC 左右，然后经过整流、滤波和调节，降至控制电子设备希望看到的电压(3.3V/5V)。

这个项目实际上仍处于[汤姆]计划的早期阶段；一个由传感器和设备组成的网络，带有一个 beagle bone 基站。我们迫不及待地想知道这个项目的下一步是什么；也许我们甚至会看到一些语音控制，就像这个史诗般的 Siri 控制的家庭自动化项目。

[via [危险原型](http://dangerousprototypes.com/2014/01/03/magic-mote-thermostat-and-wireless-temperature-sensor/)