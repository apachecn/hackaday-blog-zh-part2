# 加速 AVR 除法的详细教程

> 原文：<https://hackaday.com/2012/07/15/a-detailed-explanation-on-speeding-up-avr-division/>

![](img/96bbaad56e7c565226b7290f14d35697.png "fixedpoint")

[Alan Burlison]正在开发一个 Arduino 项目，该项目使用了一个加速度计和几个 led。当他的电路板向一边或另一边倾斜时，led 灯就会亮起，这是一个足够简单的项目，一个电脑牛仔可以在一个小时内完成，但[艾伦]——曾经的完美主义者——决定优化他的代码，以便他的加速计控制的 led 灯不会抖动。结果是[一篇壮观的博客文章](http://bleaklow.com/2012/06/20/sensor_smoothing_and_optimised_maths_on_the_arduino.html)记录了 AVR 上浮点数学和除法的陷阱。

为了消除 led 的抖动，[Alan]使用了一种被称为[的平滑算法，即指数移动平均值](http://en.wikipedia.org/wiki/Moving_average#Exponential_moving_average)。该算法使用乘法，并且通常使用浮点运算来实现。不幸的是，AVR 没有浮点运算，所以[Alan]使用定点运算——一种类似于以美分而不是美元结算支票簿的系统。

通过巧妙地使用位移位来计算缩放的平均值，[Alan]能够使定点版本比浮点算法实现快近 6 倍。在深入研究了他的定点算法的汇编之后，他能够将它的速度提高到浮点运算的 10 倍。

从[艾伦]的算术冒险中得到的启示是 AVR 上的除法运算很慢。当你意识到 AVR 没有除法指令时，这并不奇怪。当然，有时你不能避开除法，所以如果速度是个问题的话，乘以倒数并使用定点运算是个不错的方法。

当然，如果你只是使用 Arduino 作为开关，从 8 位微控制器中挤出最后一个周期有点过分。如果你正在处理图形或者需要非常快的响应时间，[Alan]给出了很多非常有用的提示。