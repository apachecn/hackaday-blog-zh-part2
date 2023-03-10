# Hack 允许 ESP-01 进入深度睡眠

> 原文：<https://hackaday.com/2015/02/08/hack-allows-esp-01-to-go-to-deep-sleep/>

基于 ESP8266 的 ESP-01 模块目前在物联网领域风靡一时，为什么不呢？大约 5 美元，它提供的功能在价格上是无与伦比的。这种收音机经常做的一件事就是耗电。因此，毫不奇怪，减少这款设备的耗电量是许多人的首要任务。[Tim]想出了一个简单的硬件[黑客让 ESP-01 进入深度睡眠](http://tim.jagenberg.info/2015/01/18/low-power-esp8266/)，有效地将其电流消耗降低到 78uA——低到足以允许电池供电部署。

当[Tim]正在努力理解 [ESP8266](https://nurdspace.nl/ESP8266) 工具链( [NodeMCU](http://nodemcu.com/index_en.html) 固件> [Lua](https://en.wikipedia.org/wiki/Lua_%28programming_language%29) 解释器> [ESPlorer](http://esp8266.ru/esplorer/) IDE)时，他意识到在 ESP-01 模块上无法访问一些重要的引脚。[Tim]在 perf 板上构建了一个开发板，让他可以访问这些引脚，同时还添加了一些装饰。我们猜测他(或其他人)会想出一个合适的 PCB 来使事情变得更容易。但真正的黑客是在 ESP-01 模块本身。[Tim]需要将 MCU 上的“睡眠后复位引脚”硬连线到复位端子。此外，还要用螺丝刀撬开指示灯！这听起来有点极端，我们建议你把烙铁拿出来。如果你是一个不幸的人，收到了发布 ESP8266 模块的[“魔法烟雾](http://hackaday.com/2015/01/08/faulty-esp8266s-release-smoke-then-keep-working/)，那么无论如何你都不需要 LED。