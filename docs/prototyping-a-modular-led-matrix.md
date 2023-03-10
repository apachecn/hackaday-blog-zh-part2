# 模块化 LED 矩阵原型

> 原文：<https://hackaday.com/2013/03/18/prototyping-a-modular-led-matrix/>

![led-matrix-modular-prototype](img/a7566f098cc02a6d1b284f49eaf250b2.png)

[Will]正在考虑制作一个滚动 LED 字幕来显示他五月份婚礼的信息。但是你得先爬才能走，所以他决定看看他能用 MAX7219 LED 驱动芯片做些什么。它们采用 DIP 封装，但 24 引脚 0.1 英寸间距的芯片最终会比他想要使用的 8×8 LED 模块更大。因此，他选择了表面贴装部件，并[旋转 PCB，使 led 模块化](http://www.mobilewill.us/2013/03/led-matrix-link-prototype.html)。

当你处理大量发光二极管时，这些驱动程序非常棒(比如[许多闪烁颜色的摩托车头盔](http://hackaday.com/2012/09/14/helmet-of-many-leds-built-for-burning-man/))。由于它们使用 SPI 进行通信，因此可以用最少的连接来链接芯片。[Will]将他的电路板设计成一边有一个公接头，另一边有一个母插座。它不仅使每个模块的对齐和连接变得简单，而且允许您随时改变主意，决定使用哪个微控制器来控制它们。在第一组测试中，他将插头插入试验板，并用 Arduino 驱动它。我们希望听到他的最新消息，届时最终的设备将会在这个重要的日子里组装完成。