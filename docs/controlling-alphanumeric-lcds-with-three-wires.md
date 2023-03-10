# 用三线控制字母数字液晶显示器

> 原文：<https://hackaday.com/2014/02/03/controlling-alphanumeric-lcds-with-three-wires/>

![shift](img/16b1c0aaaeafc546699ade7859849c55.png)

HD44780 LCD 控制器实际上是向您的下一个项目添加小文本显示的方式。如果你需要一种方法来显示几个变量，几行文本，或者给一个项目添加一个小的用户界面，你可能会使用这些并行液晶显示器中的一个。这些显示器至少需要六条控制线，如果你正在使用一个小的微控制器或者只剩下最后一个引脚，你可能要考虑用移位寄存器控制一个 LCD。

[Matteo]使用无处不在的 595 移位寄存器配置为串行到并行转换器来驱动他的 LCD。以这种方式驱动 LCD 只需要 Arduino[Matteo]选择的微控制器上的三个引脚。

对于软件，[Matteo]修改了股票 Arduino LiquidCrystal 库[并将其放在他的 Git](https://github.com/MatBenetti/LiquidCrystalS2P)上。大多数功能保持不变，但对于这个版本，LCD 只能在其四位模式下使用。这在 99%的情况下都不是问题，但是如果你需要在你的 LCD 上自定义字符，你可以随时连接另一个移位寄存器。

如果你不能为一个显示器腾出三个引脚，你可以[将它压缩到只有两个](http://hackaday.com/2013/03/11/two-wire-serial-backpack-for-glcd-screens/)，或者添加第二个微控制器作为一个[单线式接口](http://hackaday.com/2014/02/01/controlling-alphanumeric-lcds-with-two-wires/)。