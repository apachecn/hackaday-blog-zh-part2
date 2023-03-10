# Hackaday 奖参赛作品:智能低压照明

> 原文：<https://hackaday.com/2015/07/25/hackaday-prize-entry-smart-low-voltage-lighting/>

围绕物联网的一个常见主题是将中继连接到网络。它对任何事情都很有用，从打开全国各地的灯到确保你的冰箱在没有国际制冷委员会每小时两次电话的情况下仍能运转。对于他的 Hackaday Prize 项目，[Matt]正在用 ESP8266 WiFi 模块打开和关闭灯，但不是任何灯:[他正在用 ESPLux 专注于低压照明](https://hackaday.io/project/4731-esplux-smarts-for-your-downlights)。

大多数筒灯和景观灯使用 12 或 24 伏的变压器，因为[马特]想在他的灯箱中增加调光功能，他正在将低压交流电整流到 DC；PWM 输出点亮 LED 比用三端双向可控硅开关斩波交流要好得多。

使用整流器、MOSFET 和 ESP8266，ESPLux 是一个简单的构建，但该项目并不仅限于电子产品。对于这些灯的自动化和控制，[Matt]转向了 [OpenHAB](http://www.openhab.org/) ，这是一款自动化软件，可以与你用来让你的家变得智能的所有东西一起工作。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)