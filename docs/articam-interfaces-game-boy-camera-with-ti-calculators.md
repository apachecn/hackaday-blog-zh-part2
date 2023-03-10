# arricam 将 game boy 相机与 ti 计算器相连接

> 原文：<https://hackaday.com/2014/11/29/articam-interfaces-game-boy-camera-with-ti-calculators/>

克里斯托弗·米切尔(Christopher Mitchell)让德州仪器(Texas Instruments)的计算器能够通过带有 ArTICam(T1)的游戏机摄像头捕捉图像。[Game Boy Camera](http://en.wikipedia.org/wiki/Game_Boy_Camera)于 1998 年首次推出，是首批面向消费者的低成本数码相机之一。从那时起，它已经进入了相当多的项目，包括[这个基于 Atmel AT90 的早期黑客](http://hackaday.com/2009/09/23/vintage-hack-game-boy-camera/)，和[这个莫尔斯电码收发器](http://hackaday.com/2012/12/10/morse-code-transceiver-based-on-gameboy-color-camera/)。

TI 计算器不包括 Game Boy 墨盒插槽，所以[Christopher]使用了 Arduino Uno 来连接这两者。他在 Arduino-TI 计算器链接(ArTICL)库的基础上创建了 ArTICam。让 Arduino 与 Game Boy Camera 的 M64282FP 图像传感器对话被证明是很容易的，因为已经有了[代码示例。](https://code.google.com/p/avr-gameboy-cam/)摄像头传感器和 Arduino 之间的接口非常简单。用于 oddball 串行接口的 6 条数字线、一条模拟感测线、电源和地线。[Christopher]使用了一个屏蔽来焊接所有的东西，但他说你可以很容易地直接连接 Arduino Uno 的 I/O 引脚。该系统与 TI-83 Plus 和 TI-84 Plus 系列计算器兼容。抓取图像就像从计算器程序中调用 GetCalc(Pic1)一样简单。

所以，如果你有一个旧的计算器，试着享受一下 128×123 像素的灰度吧！