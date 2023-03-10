# 用 LED 灯带上的电机更换 LED

> 原文：<https://hackaday.com/2013/09/11/switching-leds-with-motors-on-a-led-strip/>

[![](img/30b1b7542cf4b696ff53ddd3140b9c14.png)](http://hackaday.com/wp-content/uploads/2013/09/tumblr_inline_ms73u9vggu1qz4rgp.jpg)

Hackaday 校友 Caleb Kraft 向我们透露了他在今年的开放硬件峰会上看到的一个不错的黑客技术。这是一个由 LED 条制成的[柔性触觉条](http://citizengadget.com/post/59494035738/led-light-strip-hacked-for-haptic-motors)。

便宜的柔性印刷电路板不容易找到，所以[Jacob]基本上是用无轴振动电机来切换他的条带中的所有 RGB LEDs。LED 使用 WS2801 LED 驱动器寻址，因此黑客还包括短路电流反馈电阻。因此，电机将使用尽可能多的电流，因为司机可以给和[雅各布]可以单独驱动每个电机。对他来说幸运的是，已经有一个名为 fastSPI 的 Arduino 库来驱动条带，所以他很快就成功地制作了一个不错的触觉设备。如果你想知道，你可以驱动的最大电机数量是 32。

我们自己的[Eric Evenchick]在 OHS 的时候也看到了很多很棒的项目演示。

[via [EE Times](http://www.eetimes.com/author.asp?section_id=36&doc_id=1319443)