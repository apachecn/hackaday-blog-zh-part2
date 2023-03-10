# 定制数码管 PSU 是一个良好的 PCB 设计的教训

> 原文：<https://hackaday.com/2014/05/11/custom-nixie-tube-psu-is-a-lesson-in-good-pcb-design/>

![Nixie HVPSU](img/901d6501c5daf025ac3fd37592b946dc.png)

[Jan Rychter]厌倦了无法为他的数码管项目找到合适的电源，所以他决定自己设计。[Jan]开始围绕 [MAX1771](http://datasheets.maximintegrated.com/en/ds/MAX1771.pdf "MAX1771") (PDF) DC-DC 控制器进行设计，但很快发现他有稳定性问题。即使在七次董事会修订后，他仍然经历着不受控制的行为。他最终放弃了 MAX1171，改用德州仪器 [TPS40210](http://www.ti.com/product/tps40210 "40210") 。经过三次以上的电路板设计，他终于有了适合自己的东西。[Jan]承认他的设计可能并不完美(可能会愚弄我们！)，但他想把它作为开源硬件向全世界发布，以回馈社区。

[Jan]努力工作的最终结果是一块 5cm×5cm 的电路板，它可以从一个 12V 电源产生四个独立的输出电压。其中包括用于数字逻辑的 3.3V 和 5V 输出，以及用于谢妮管的 220V 输出和用于迪卡龙的 440V 最大输出。该电路还具有若干安全特性，包括过流保护、热关断和慢启动。请务必查看[【Jan 的】网页](http://jan.rychter.com/high-voltage-power-supply-for-nixie-tube-projects "Jan's webpage")查看这款出色电路的原理图和技术信息。

需要一些谢妮电子管来配合电路吗？我们知道一些[资源](http://hackaday.com/2009/12/18/need-to-source-nixie-tubes/ "Nixie sources")供你查阅。或者你也可以一直只让[建造](http://hackaday.com/2013/11/07/homemade-nixie-tubes/ "DIY nixie tubes")你的[自己的](http://hackaday.com/2010/07/27/making-nixie-tubes-at-home/ "DIY nixie tubes")。你将如何在你的下一个项目中使用这个板？