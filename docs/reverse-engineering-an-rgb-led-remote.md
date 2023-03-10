# 对 RGB LED 遥控器进行逆向工程

> 原文：<https://hackaday.com/2012/05/10/reverse-engineering-an-rgb-led-remote/>

![](img/b715d1337ed6478da8e58edf0abe4cdb.png "LED")

为了在他的地下室增加一些情调照明，[Mohonri]找到了一个能够控制几个 RGB LED 灯的红外无线遥控器。这种遥控器的唯一问题是无法通过壁挂式面板甚至电脑来控制它。显然，这不能代表如此奢华的地下室，所以[Mohonri]做了合理的事情，对其中一个遥控器进行了逆向工程。

构建从拆开遥控器开始，并弄清楚它是如何工作的。[Mohonri]找到了小型红外 LED 发射器，并连接了示波器来捕捉一些数据。经过一系列的试验和错误，以及相关文档的[大力帮助，他拥有了整个按钮矩阵——以及 LED 灯条可用的功能——可通过墙板或计算机输出。](http://www.sbprojects.com/knowledge/ir/index.php)

[Mohonri]还没有完成他的建造；这只是逆向工程和文档阶段。不过现在，通过一个 Arduino、一台电脑，甚至一个插在耳机插孔上的小红外 LED 的 Android/iOS 设备，控制 RGB LED 灯条应该不难。