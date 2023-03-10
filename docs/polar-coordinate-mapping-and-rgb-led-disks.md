# 极坐标映射和 RGB LED 盘

> 原文：<https://hackaday.com/2015/05/04/polar-coordinate-mapping-and-rgb-led-disks/>

上周，Adafruit 发布了 DotStar RGB LED 盘，这是一个直径为 240 毫米的盘，装有 255 个可单独寻址的 RGB LED。因为 blinkey glowey 项目是最好的项目，[亚当]必须有一个。[他的测试在 blinkey LED 的世界里打开了一些有趣的可能性](http://maniacallabs.com/2015/05/04/review-code-adafruit-dotstar-disk/)，包括一个*极坐标*显示器，非常适合低分辨率游戏和 LED 时钟。

[亚当]发现磁盘足够明亮和 glowey，但有两个问题。第一个是 DotStar 磁盘输入上的 JST SM 连接器；由于磁盘上有 255 个 led，它的最大功耗超过 10A，而连接器只能提供 7A 而不会变得不合理地热。其次，在圆盘的外缘没有 60 个发光二极管，限制了它作为时钟的应用。

DotStar 磁盘还有一个问题，直到你意识到它实际上是一个极坐标显示器。RGB LED 库通常是为条带或矩阵编写的，而不是圆形。led 按顺序排列在向内螺旋的 DotStar 盘上，在摆弄了一些可怕的代码后，[Adam]意识到他可以只通过像素与中心的距离和与连接器的角度来控制像素。这使得绘制圆更容易，但它也打开了一些有趣的应用显示；圆形乒乓会很酷，LED 时钟是蜜蜂的膝盖。