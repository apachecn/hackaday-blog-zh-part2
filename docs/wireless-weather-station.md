# 无线气象站

> 原文：<https://hackaday.com/2015/06/22/wireless-weather-station/>

高中生[弗拉德]花了大约一年时间建造他的电池供电的无线气象站。一路走来，他不仅学到了很多有用的技能，还设法在博客上记录了自己的进步。

该站测量温度、湿度、压力和电池电压，他计划很快增加风速、风向和降雨量传感器。它通过太阳能电池板供电，可以在充满电的电池上运行整整一个月。传感器模块将数据传输到与计算机相连的远程接收器，并从那里发布到互联网上。使用 BMP180 测量大气压力，DHT22 提供温度和湿度值。发射和接收部分之间的链接使用 433MHz 超外差射频套件，使[Vlad]的范围达到 50 米。发射器和接收器端有一个 ATMega328。他每 12 分钟测量一次，并使用 [Rocket Scream 低功耗库](http://www.rocketscream.com/blog/2011/07/04/lightweight-low-power-arduino-library/)将微控制器置于低功耗模式。5W、12V 太阳能电池板通过基于 LM317 的充电电路为 6V 铅酸电池充电。这确保了即使太阳能电池板没有接收到最佳辐射，电池也能充电。一小时的阳光提供的电量足以让它持续工作两天。即使没有阳光，充满电的电池也能让它运行一个月。

服务器软件由两部分组成。第一个将串行数据推送到 mySQL 数据库。这是用 Visual Studio C#编写的，使用了来自 Oracle mySQL connector 的帮助。第二部分将 mySQL 数据库中的条目发布到 web 服务器。这是用 php 编写的，并使用 [Libchart](http://naku.dohcrew.com/libchart/pages/introduction/) 进行绘图。他在自己的博客上有[代码](http://denialmedia.ca/files/SWS.zip)、原理图、[零件清单](http://denialmedia.ca/parts-for-my-new-project-weather-station/)和许多其他可供下载的信息。他的待办事项列表上还有几项未完成，所以如果你有任何建议，请在下面发表你的评论。