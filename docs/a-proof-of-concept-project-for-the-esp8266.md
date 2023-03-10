# ESP8266 的概念验证项目

> 原文：<https://hackaday.com/2014/09/17/a-proof-of-concept-project-for-the-esp8266/>

自从我们第一次听说用于 micros 的便宜得不可思议的 WiFi 适配器 ESP8266 以来，还不到一个月。从那以后，订单慢慢地从中国的港口流出，流向世界各地修补匠的工作台。[最后，我们有一个使用这个模块](http://zeflo.com/2014/esp8266-weather-display/)的工作项目。它可能只是一个显示当前天气状况的显示屏，但这是一个开始，只是这个模块能做什么的一个提示。

自从 ESP8266 进入普通经销商的店面以来，翻译 hackaday.io 和 nurdspace wiki 的数据表已经花费了大量精力。该模块确实对简单的 AT 命令做出响应，并且通过正确的代码，可以从互联网上获取少量数据。

代码从[openweathermap.org](http://openweathermap.org/api)请求数据，并在一个小的 TFT 显示屏上显示当前的温度、压力和湿度。整个事情是由一个 Arduino 驱动的，所以对于任何想要一个便宜的方式把 Arduino 项目放到互联网上的人来说，这就是你要做的。