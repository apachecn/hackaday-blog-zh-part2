# 使用工作台工具测试新显示器

> 原文：<https://hackaday.com/2012/06/29/using-your-bench-tools-to-test-a-new-display/>

![](img/9e99e86450452f20ddb3c163274d652a.png "bench-tools-to-test-a-new-display")

使用新零件时，通常需要花点功夫来获得信心。[Glitch]得到了这个由 Sabernetics 制造的有机发光二极管显示器，并想在围绕它建立一个项目之前尝试一下。他抓住他的巴士海盗，帮助了解新零件的来龙去脉。

96×16 点阵显示器使用 i2c 协议，引脚数非常少(六个引脚:接地、复位、时钟、数据、片选和电压)。由于 Bus Pirate 为您提供了对 i2c 的命令行式访问，所以这是首次测试的自然选择。事实上，对于大多数项目来说，该工具已经成为该协议的首选设备。

首先发送的命令是驱动显示器的 SSD1306 的配置值。这些参数配置对比度、电压转换和显示器通电所需的其他重要值。它突然活跃起来，显示随机像素，因为 RAM 尚未初始化。随着这一成功,[Glitch]转向了总线盗版者的脚本能力，并最终开发出一个 Python 脚本来驱动上面的演示。现在他知道了他需要的命令，为微控制器驱动程序写代码就容易多了。