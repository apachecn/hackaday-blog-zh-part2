# 受不了你吵的风扇？我有个计划，伙计

> 原文：<https://hackaday.com/2014/02/28/cant-stand-your-noisy-fan-heres-a-plan-man/>

![](img/64d1271515a76ea0ed5ae3514391830e.png)[Brian]非常喜欢他的 GW Instek GPC-1850D 电源，但是它的噪音太大，干扰了他的音频项目。这东西很好用，所以他决定[根据使用水平调节风扇的速度](http://www.briandorey.com/post/psu-temperature-monitor.aspx)来拯救他的理智。

一旦[Brian]打开盖子，他发现它实际上有四个独立的散热器:一个用于桥式整流器，一个用于三个输出通道上的每个功率晶体管。散热器彼此电气和热隔离，并根据所使用的通道改变温度。

[Brian]和他的同事有几个来自以前项目的微芯片 MCP 9803 温度传感器，所以他们在每个散热器上放了一个。最棒的是它们的地址选择引脚，这使得它们四个可以一起坐在通往 Arduinoville 的 I C 总线上。每个传感器都是绝缘的，并用一块 meccano 和少量导热膏固定在散热片上。

[Brian]使用 Arduino Mini 并在条形板上构建电路。风扇以 24V 运行，所以他通过 7805 与 Arduino 共享。他用来自 Arduino 的 PWM 通过 MOSFET 控制风扇的速度。Arduino 从每个传感器读取数据，并确定哪个传感器最热。[Brian]想要风扇一直运转，所以他设置了 20%的基本速度。当散热器温度达到 30°C/86°F 时，风扇转速将提高到 40%。此后，速度以 5°C/9°F 的间隔增加，直到在 65°C/149°F 时达到最大速度。

你可以从[【布莱恩】的回购](https://github.com/briandorey/PSU-Temperature-Monitor)中抓取代码和原理图。如果你想研究你的散热器，先建造[这个散热器测试器](http://hackaday.com/2014/01/29/heatsink-tester-shows-thermal-resistance-isnt-futile/)。