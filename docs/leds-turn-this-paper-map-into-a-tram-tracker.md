# 发光二极管将这张纸质地图变成电车追踪器

> 原文：<https://hackaday.com/2014/09/15/leds-turn-this-paper-map-into-a-tram-tracker/>

公共交通可以是一件美好的事情。如果火车晚点，这也很烦人。如今，许多公共交通系统都与互联网相连。这意味着你可以使用电脑或智能手机随时检查你的火车是否会准时。[Christoph]想为奥地利林茨的 Devlol hackerspace 更进一步，所以他为自己建造了一个电子跟踪系统。

[Christoph]从一张火车系统的纸质地图开始。它被放在一个普通的相框里。然后，[Christoph]将一系列 BulletPixel2 LEDs 并联在一起。[bulletpixel 2](http://samuraicircuits.com/merch/index.php?id_product=58&controller=product "BulletPixel2")led 是 8 毫米三色 led，还包含一个小型控制器芯片。这使得它们可以用一根线串行控制。这类似于一个 RGB LED 灯条，只是没有实际的灯条。[Christoph]使用了 50 个 led 灯。led 沿着三条主要的火车线路安装在相框中；红色、绿色和蓝色。LED 的颜色明显对应于火车线的颜色。

火车位置数据是使用 Raspberry Pi 从互联网上提取的。为了保持地图的准确性和最新性，必须不断提取信息。Raspberry Pi 然后与 Arduino Uno 通信，Arduino Uno 用于实际控制 led 串。这些电子产品都可以藏在相框后面，看不见。最终产品是用于当地火车系统的光滑的“雷达”。