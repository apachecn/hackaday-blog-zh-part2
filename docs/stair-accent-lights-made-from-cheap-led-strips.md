# 由廉价 LED 灯条制成的楼梯强光灯

> 原文：<https://hackaday.com/2012/04/13/stair-accent-lights-made-from-cheap-led-strips/>

![](img/ca89709c8a9e77f6715b17f76da4a368.png "led-strips-for-your-stairs")

我们真的很喜欢[Geert]为他的楼梯采用重点照明。他建造了自己的 [LED 通道，安装在每一级台阶的圆角](http://geertvw.blogspot.com/2011/12/leds.html)下方。他使用的 LED 灯条实际上相当便宜。它们是 RGB 版本，但像素不可单独寻址。这意味着，这种条带没有将驱动器集成到条带中(通常是那些使用 SPI 传输颜色数据的驱动器)，而是只有一个电源轨和三个颜色接地轨。十米长的带子花了他不到四十美元。

他确实希望能够单独处理每个步骤，以及混合和匹配颜色，因此他设计了上面看到的驱动板，使用一组 TLC5940 LED 驱动器。这些由 Arduino 控制，Arduino 处理颜色变化和动画。它最终将包括传感器，在你上楼时影响发光二极管。每一条都安装在一个角形支架上，它们通过电话延长线连接回驱动板。