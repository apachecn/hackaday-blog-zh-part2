# I2C 黑客:如何将时钟拼接成芯片选择

> 原文：<https://hackaday.com/2015/07/27/i2c-hacks-how-to-splice-clocks-into-chip-selects/>

有时，您需要将三个、四个或更多相同的 i2c 器件连接到一个通用微控制器。也许你正在考虑用 8 个 MAX6955 16 路数字驱动器驱动 128 个七段显示器，或者也许你有一个充满关节的机器人，每个关节都需要一个 BNO055 惯性传感器来进行角度估计。(见上。)哎呀！在这两种情况下，你最好的选择可能是一个愚蠢的 I C 设备，它可以为你做大部分的工作。问题？对于单条 I2C 总线，协议中没有定义连接两个或更多具有相同地址的设备的标准方式。开枪！连接三个 BNO055 IMUs 或八个 MAX6955s 并结束一天的工作会很方便。幸运的是，有一个变通办法。

我们在过去已经看到了一些解决这个问题的聪明绝招。[【Marv G’s】方法](http://hackaday.com/2015/03/27/using-i2c-addresses-as-chip-selects/)涉及使用外部引脚在设备的默认地址和备用地址之间切换。这种方法虽然聪明，但它假设设备( *a* )有一个备用的 I C 地址，并且( *b* )有一个外部引脚用于切换该地址。

我将介绍另外两种方法，让您的微处理器和您的一套相同传感器开始对话。第一种是“巧妙的技巧”，但是对于广泛使用来说有点不切实际。第二个更有生产价值——你可以幸灾乐祸地向你的老板炫耀！事不宜迟，让我们从 M *方法 1* 开始。

最后，如果你想继续下去，可以在 [Github](https://github.com/Poofjunior/i2c_demultiplexing_demo) 查看源代码。

[https://www.youtube.com/embed/ju89RUWVULE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ju89RUWVULE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 测试设置:

[![cube_details](img/7121094aaddbe0078d5359ee8f65ff27.png)](https://hackaday.com/wp-content/uploads/2015/07/cube_details.png)

在这两种方法中，我使用相同的传感器设置来检查每个电路的行为是否正确。我正好有一堆多余的 BMA180s 在板凳上，所以我推出了一个基于这些芯片的例子。过去， [BMA180](https://www.sparkfun.com/products/retired/9723) 是一种非常常见的三轴数字加速度计。它有一个带两个可选地址的 I2C 接口。出于这个例子的目的，我用相同的地址固定它们。我已经在我的丙烯酸“测试立方体”的相互垂直的轴上安装了三个这样的家伙，我正在读取每个芯片的 Z 轴。在这种配置中，当数据从我的串行端口窗口飞过时，我可以很容易地从相应的传感器中挑出重力矢量。如果我能唯一地寻址每个传感器并读取数据，我就有了一个工作电路。

## 方法 1:将时钟拼接到片选中

这个方法向 SPI 倾斜，因为它的行为方式非常相似。如果您对 SPI 感到生疏，这里有一个快速回顾。

### 快速 SPI 点心:

像 I C 一样，SPI 是另一种与多个从机共享时钟和数据线的协议。然而，不同之处在于与这些共享同一总线的设备通信的寻址方案。借助 SPI，虽然时钟和数据线是共享的，但器件通过单独的*片选* (CS)线寻址。

[![SPI_three_slaves](img/6cc8217064a2a35f315ddb2d1897913f.png)](https://hackaday.com/wp-content/uploads/2015/07/spi_three_slaves.png)

Image Source: [Wikipedia](https://en.wikipedia.org/wiki/Serial_Peripheral_Interface_Bus)

主微控制器为每个器件专用一个唯一的输出引脚(本图中的~ ~*SS1*、~ *SS2* 和~ *SS3* )。当主控微处理器想要与一个设备对话时，它通过将该设备的*片选*输入引脚拉至逻辑低电平来断言该引脚，对话通过数据总线开始。当*片选*为低电平时，相应的从机监听总线上的数据。与此同时，所有其他器件通过将其总线引脚保持在*高阻抗*状态，忽略主机与其所选从机之间的对话。

### 给予 I C 自己的芯片选择:

对于 I2C，时钟(SCL)和数据(SDA)线仍然在所有 I2C 从设备之间共享，但寻址方案是通过发送总线上所有设备都能听到的消息来实现的。为了选出共享总线上的一个器件，主机首先向下传递它想要与之通信的从机的地址，之后该从机应答应答，所有其它从机忽略随后的数据，直到两个数据传输都完成并且总线被“释放”。

[![i2c_normal_operation](img/13f94290b3aeaabf8d4e9a9a863d19da.png)](https://hackaday.com/wp-content/uploads/2015/07/i2c_normal_operation1.png)

因为我们有多个具有共享地址的设备的问题，理论上，当主设备传递它们的共享地址时，所有这些设备的*都将回复，并且主设备没有办法挑出单个设备。实际上，这种行为在 I2C 协议上是没有定义的*。**

 *[![i2c_bad_operation](img/b9b863689f2a38ce9637ef32a342aa94.png)](https://hackaday.com/wp-content/uploads/2015/07/i2c_bad_operation1.png)

哎呀！当我们偏离定义的行为时，任何事情都会发生，所以我们在实践中尽量避免这些事情。

## 解决办法？

根据 I C 规范，只要时钟线(SCL)保持高电平，I C 从设备就会*忽略*数据*线(SDA)上的*变化。在这种方法中，我将 SCL 线“分割”成多条 SCL 线，这样每个共享的 I C 设备都有自己的 SCL。通过有选择地一次一个地将时钟重新路由到每个 I C 设备，我基本上已经将 SCL 线变成了“芯片选择”

为了切断时钟线，我需要一个多路分解器。多路分解器(或解码器)获取逻辑输入，并基于二进制选择线将其重新路由到几个输出之一。

 [![demux](img/56005155c1623607cc4d7457fa9df14e.png "demux")](https://hackaday.com/2015/07/27/i2c-hacks-how-to-splice-clocks-into-chip-selects/demux/)  [![i2c_demultiplexing_demo](img/1625523f7629139bccd26048b69d1743.png "i2c_demultiplexing_demo")](https://hackaday.com/2015/07/27/i2c-hacks-how-to-splice-clocks-into-chip-selects/i2c_demultiplexing_demo/) 

为了完成这项任务，我加入了 74AC11138 八路解复用器。它速度很快，能够以兆赫的速率切换，其输出默认为逻辑高电平。第二点很方便，因为空闲的 SCL 线路也默认为逻辑高电平。

设置如上面的简化示意图所示。在里面，我用了一个 Teensy 3.0 来冒充 I C 总线主。在 Teensy 的右边是相同芯片的集合，在这种情况下是 BMA180 加速度计。中间是 74AC11138 八路解复用器。

## 这种方法的缺点:

不过，这种技术有一个小缺点，它不支持 I C 的*时钟拉伸*功能。退一步说，这种方法假设 SCL 线本质上是单向的，只由 I2C 总线主控器控制。换句话说，我们假设 SCL 线上的数据只从主设备发送到从设备，而不是从主设备发送到从设备。然而，如果你的 I C 从设备实现了时钟拉伸，这个假设就不成立了。

### 什么是时钟拉伸？

*时钟拉伸*是由 I C 协议定义的一种方法，在这种方法中，芯片需要“为自己赢得更多时间”，并将 SCL 线保持在低电平，因此，向主机发出信号，表示它尚未准备好接收即将到来的数据。在这种情况下，从机主动控制 SCL 线，并且这恰好是数据从从机到主机沿着 SCL 线向上移动的唯一情况。在主设备和我们的一组相同从设备之间的解复用器的设置中，如果这些从设备碰巧实现了*时钟拉伸*，它们将无法向主设备发回时钟拉伸信号，以表明它们没有准备好接收数据。也就是说，*时钟延伸*在 I C 兼容设备中是一个非常罕见的功能，所以这种方法很可能在现在推出的许多芯片中行得通。

## 下周更多

*方法 1* 到此为止。感谢收听，下周再来看看解决这个问题的更专业的方法。*