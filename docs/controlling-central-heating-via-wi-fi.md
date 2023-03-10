# 通过 Wi-Fi 控制中央供暖

> 原文：<https://hackaday.com/2015/02/27/controlling-central-heating-via-wi-fi/>

如果你曾经住在一栋有手动控制中央供暖系统的建筑里，你可能会理解[马丁]这次黑客行动的动机。这些供暖系统通常有老式的阀门来控制散热器。没有鸟巢支架，没有恒温器，只有一个旋钮。

为了解决这个问题，【马丁】建造了一个[支持 Wi-Fi 的恒温器](http://harizanov.com/2015/02/wifi-thermostat-with-weekly-scheduler/)。这一令人印象深刻的构建将基于 [ESP8266](http://hackaday.com/tag/esp8266/) Wi-Fi 微控制器的定制 PCB 和基于[开放式恒温调度器](https://github.com/emoncms/development/tree/master/experimental/control/open_thermostat_scheduler)的移动友好网络 UI 结合在一起。该项目的 web 服务器在 ESP8266 上是完全独立的。

为了取代手动值，[Martin]使用了一家名为 HERZ 的瑞士公司的热电致动器。这是由一个继电器驱动的，该继电器由 ESP8266 微控制器控制。根据时间表和测得的温度，致动器让流体流过散热器并加热房间。

作为奖励，该设备支持 [NTP](http://www.ntp.org/) 获取时间， [MQTT](http://en.wikipedia.org/wiki/MQTT) 发布实时数据，以及 [ThingSpeak](https://thingspeak.com/) 记录和绘制历史数据。源代码和设计文件可以在知识共享许可下获得。