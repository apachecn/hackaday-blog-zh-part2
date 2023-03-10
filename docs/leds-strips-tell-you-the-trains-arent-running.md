# 发光二极管带告诉你火车没有运行

> 原文：<https://hackaday.com/2015/05/08/leds-strips-tell-you-the-trains-arent-running/>

[詹姆斯]是伦敦地铁的常客，这是一个无法避免故障和延误的地铁系统。他想要一种方法来轻松地判断是否有任何列车被中断，并且[由于一些 led](https://unop.uk/dev/train-disruption-indicator-with-a-blinky-tape-rgb-led-strip-and-raspberry-pi/)，他现在可以一目了然地获得这些信息，而不必先查看网页。

受到 FT EngineeringBlinky Tape 项目的启发，【James】认为他可以使用同样的可寻址发光二极管带来显示关于电子管的信息。Raspberry Pi B+从伦敦地铁的 TfL API 收集数据，并对数据进行一些计算。如果有延迟，灯带相应部分的发光二极管就会闪烁，提醒用户只需匆匆一瞥就能发现问题。

该项目是许多显示数据的项目之一，当你走出房子时，你会发现这些数据，而不必看电脑或智能手机。我们最近展示了一个[艺术灯，它显示未来 12 小时的天气预报](http://hackaday.com/2015/04/29/use-a-lamp-to-see-into-the-future/)，还有一个[伞架](http://hackaday.com/2012/11/15/an-umbrella-stand-that-tells-you-the-weather-forecast/)也做了同样的事情。有了 led 和一个好的 API，很多事情都是可能的！

[https://player.vimeo.com/video/127014091](https://player.vimeo.com/video/127014091)