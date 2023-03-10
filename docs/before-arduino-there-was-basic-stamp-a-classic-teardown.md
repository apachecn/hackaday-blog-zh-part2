# 在 Arduino 之前有一个基本的印记:经典的拆卸

> 原文：<https://hackaday.com/2015/08/27/before-arduino-there-was-basic-stamp-a-classic-teardown/>

微控制器在 Arduino 之前就已经存在，任何人都可以编程并闪烁 LED 的设备在第一次 Maker Faire 之前就已经存在。这可能会让一些人感到惊讶，但对其他人来说，PICs 和 68HC11s 将继续作为第一个受欢迎的微控制器，出现在从玩具到微波炉的所有东西中。

Arduino 甚至不能声称它是第一个用户友好的微控制器开发板。这个头衔属于谦逊的基本邮票，这是一个在 20 世纪 90 年代初推出的四个组成部分的董事会。我最近设法得到了一套原始的基本邮票。这是拆卸和介绍第一个用户友好的微控制器开发板。就当这是一次回忆之旅吧，它向我们展示了在过去的二十年里电子产品市场已经走了多远，也让我们看到了我们还有多远的路要走。

[![The Basic Stamp 1\. A Simple circuit with just a microcontroller, an EEPROM, crystal, and brownout circuit.](img/95667fd43934f349d5edd60eaff71d83.png)](https://hackaday.com/wp-content/uploads/2015/08/basicstamp.jpg)

The Basic Stamp 1\. A Simple circuit with just a microcontroller, an EEPROM, crystal, and brownout circuit.

### 拆卸

我工作台上的基本邮票套件是 1993 年制作的，建议零售价为 139 美元。经通胀调整后，这相当于 2015 年的近 230 美元。你在基本邮票初学者工具包里得到什么？一张邮票、一封程序员电报和数量惊人的文档。

基本邮票是一个极其简约的板，做的刚刚够闪烁的 LED，阅读按钮，或驱动液晶显示器。在官方文档中，只有少数几个部分:一个微控制器、一个带有几个字节内存的 EEPROM、一个晶体和一个稳压器。

该 [PIC16C56XL](http://www.microchip.com/wwwproducts/Devices.aspx?product=PIC16C56) 是该装备的大脑，具有 1.5 千比特的闪存和 *25 字节的 RAM*。按照现代标准，它很小；最接近的现代模拟将是当时的，它本身并不是一个非常新的芯片。微芯片最小和最新的芯片是 [PIC12LF1522](http://www.microchip.com/wwwproducts/Devices.aspx?dDocName=en559859) ，具有两倍的闪存和十倍的 RAM。当使用基本印章时，我们正在处理一个旧的微控制器

[![Like the Arduino, it was encouraged to use the Basic Stamp in product design.](img/6020602d3c372305669874629b8ff962.png)](https://hackaday.com/wp-content/uploads/2015/08/basicstampdesign.jpg)

Like the Arduino, it was encouraged to use the Basic Stamp in product design.

其他组件包括一个 [93LC56](http://www.microchip.com/wwwproducts/Devices.aspx?product=93LC56) 串行 EEPROM。除此之外，还有一个 4MHz 谐振器，一个 5V 线性稳压器，一个晶体管和几个电阻用于“掉电”电路。电源由焊接在板上的 9V 电池连接器提供。

基本邮票的电子设计很简单，是的，但有一个疯狂的方法。您为基本印章编写的代码存储在 256 字节的 EEPROM 中。PIC 上的 PBASIC 解释器读取该代码，忠实地执行命令，使 LED 闪烁或在 LCD 上显示字符。微控制器上实际上没有存储用户代码。

[![BasicStamp](img/37035fa2506fc3fa650331fef752fd78.png)](https://hackaday.com/wp-content/uploads/2015/08/basicstamp.png)

### 编程；编排

编程环境怎么样？这是在 DOS 外壳中运行的一个可执行文件。对系统的要求只有一台 IBM PC 或兼容的，DOS 2.0+，128k 的内存和一个磁盘驱动器。微薄的要求，但这不是一些将运行在您的现代 Windows 工作站；它需要一个合适的并行端口。

对于一个 IDE，基本的 Stamp 编辑器可以与早期的 Arduino IDEs 相媲美；Alt+R 运行连接电脑的图章上的程序，Alt+L 加载一个程序，Alt+S 保存一个程序，Alt+Q 退出编辑器。

PIC 上实现的 BASIC 语言很少，但是它做了你所期望的一切；单个引脚可以设置为输入和输出，按钮去抖，PWM 功能融入语言中。

[![Basic Stamp Ad](img/2cd25acfb3fabf75a9c5e8ee8f2727bf.png)](https://hackaday.com/wp-content/uploads/2015/08/basicstamp1.png)

An ad for the Basic Stamp. From High Tech Entrepreneur, October/November 1993\. Ads had text in the past.

### 语境

基本邮票现在被认为是过去缓慢、不方便的人工制品。没人用它，你唯一能找到它的地方是物理或电子教室的后柜里。这是对一项仍然令人印象深刻的技术的难以置信的伤害，用我们现代的期望来回顾基本邮票是一种难以置信的偏见。

在基本邮票之前就有微控制器开发平台，但这些都是工程工具，与邮票相比非常昂贵。电子爱好者的开发平台也在邮票之后出现:Micromint Domino 将整个开发平台装进了一个长方形的塑料砖块中。尽管该平台存在缺点，但这些设计都无法与基本邮票的受欢迎程度相媲美。

Arduino 受到了很多憎恨。批评者说，它对于适当的嵌入式编程来说级别太高，对于现代工作流来说级别不够高，基于旧的过时芯片，没有现代 ARM 微控制器的功能，IDE 一团糟。尽管 IDE 功能更差，内存不足，处理器速度较慢，但 Basic Stamp 被证明非常受欢迎。事实上，你可以在任何一家电台买到一套基本的邮票开发工具，这可能也不会影响它的流行。

现在，有了我们花哨的 ide、mbed 微控制器、强大的 arm 和庞大的库，Basic Stamp 的易用性仍然无法与之匹敌。它可能是缓慢的，过时的，但我们所有人都欠这个基本印记一大笔债，因为它将整整一代人引入了嵌入式编程、微控制器和电子修补的世界。