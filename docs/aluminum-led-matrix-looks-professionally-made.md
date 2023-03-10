# 铝制 LED 矩阵看起来很专业

> 原文：<https://hackaday.com/2014/04/22/aluminum-led-matrix-looks-professionally-made/>

![IMG_1073](img/90327fe072cb1fd0541c9356a7904701.png)

[大卫·唐利]想做一个 LED 矩阵已经有一段时间了，他决定最终[扣动扳机](http://www.mrdonley.com/photos)——毕竟，这么多 LED 肯定不便宜！

他使用一组 16 个 Adafruit 8×8 NeoPixel LED 矩阵(价值约 600 美元的 LED)和一个 BeagleBone Black 来控制它们。为了安装 LED 矩阵，他买了一块 6061-T6 铝片，有两个目的——一是作为一个巨大的散热器，二是看起来很酷。他所要做的就是在薄板上钻一些孔，然后用 3M 300LSE 双面胶将新像素粘在表面上。结果是一个看起来干净和专业的无边框显示器。

为了给阵列供电，他使用了 5V 90A 的电源——在全亮度下，这些 led 可以消耗大约 325W，或 5V 时 65A！从 GitHub 上的开源代码[led scape](https://github.com/osresearch/LEDscape)中做笔记，他制作了自己的软件来控制显示器——休息后留下来看看它的运行。

[https://player.vimeo.com/video/92473020](https://player.vimeo.com/video/92473020)

一个更便宜的版本(虽然不是全彩色的)可以使用[中国 LED 阵列，价格只有](http://hackaday.com/2013/10/26/an-impressively-large-led-matrix/)的几分之一——96 x 48 分辨率！