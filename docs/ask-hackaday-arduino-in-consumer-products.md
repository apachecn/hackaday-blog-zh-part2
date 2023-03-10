# 问问 Hackaday:消费产品中的 Arduino

> 原文：<https://hackaday.com/2015/07/15/ask-hackaday-arduino-in-consumer-products/>

与那些自认为是核心工程师的人交谈，你可能会听到“Arduinos 是给 noobs 用的”或其他类似的废话。这些反对者认为这个平台是一个简化的、价格过高的、被过度宣传的工具，它让你闪烁几个发光二极管，甚至可能读取一两个传感器。他们可能会说 Arduino 非常适合高中项目和在车库里修修补补的 EE 爱好者，但真正的工程是用 ARM、x86 或 PICs 完成的。你猜怎么着？这三种架构都有 Arduino 兼容板。下面你可以在 [DUE](https://www.arduino.cc/en/Main/arduinoBoardDue) 、 [Galileo](https://www.arduino.cc/en/ArduinoCertified/IntelGalileo) 和 [Fubarino SD](http://fubarino.org/sd/index.html) 电路板上看到三个例子。

 [![Arduino DUE uses Atmel ARM](img/59db983d79d62ab8e4ae01fa4bb154af.png)](https://hackaday.com/2015/07/15/ask-hackaday-arduino-in-consumer-products/arduinodue_front/) Arduino DUE uses Atmel ARM [![Arduino Galileo uses Intel x86](img/b5eb4422e24c0479e3713637212a51b1.png)](https://hackaday.com/2015/07/15/ask-hackaday-arduino-in-consumer-products/intelgalileo_fabd_front/) Arduino Galileo uses Intel x86 [![Fubarino SD uses PIC32](img/4ee55e70c8a3025d716054ea74b180d0.png)](https://hackaday.com/2015/07/15/ask-hackaday-arduino-in-consumer-products/fubarinosd1/) Fubarino SD uses PIC32

这种对 Arduino 的态度主要是出于无知而存在。因此，让我们打破一些可能仍然潜伏在一些 EEs 中的神话和先入为主的偏见，然后谈论 Arduino 超越制造商的能力。

## Arduino 不是 Uno

当一些人听到“Arduino”时，他们会想到那个可以插入 9v 电池并开始制作东西的蓝色小板子。虽然这在技术上是正确的，但事实远不止如此。

1.  一个 Arduino Uno 只是一个 AVR 开发板。AVR 类似于 PICs。当一些人说“我使用 PIC 作为主处理器”，这是否意味着他们将整个 PIC 开发板嵌入到他们的项目中？当然不是。Arduino 也是如此(大多数情况下)，设计方式与任何其他微控制器相同——
    *   使用开发板制作、创建和调试。
    *   准备就绪后，将处理器移至专用主板。
2.  使 Arduino 成为“Arduino”而不仅仅是 AVR 的是引导装载程序。因此:
    *   Atmega328P 是一种 AVR 处理器。
    *   带有 Arduino 引导加载程序的 Atmega328P 就是 Arduino。
3.  引导程序允许你用 Arduino IDE 对 AVR 进行编程。如果您从 AVR 中移除引导程序，现在您就有了一个 AVR 开发板，可以使用您喜欢的语言用 AVR Studio 进行编程。

## 没有特殊的 Arduino 语言

![Arduino "blink" sketch should run on any Arduino compatible board.](img/bd458bf3b296261293d5d5fae0ae7238.png)

Arduino “blink” sketch should run on any Arduino compatible board.

是的，我知道他们称之为草图，这很傻。但事实是它只是 c++。同样的 c++你可以用来编写你的图片。bootloader 允许 IDE 调用函数，这使得编写代码变得容易，也让 Arduino 获得了易于使用的名声。但是不要让“容易”愚弄了你。它们是真正的 c/c++函数，传递给真正的 c/c++编译器。事实上，任何 c/c++结构都可以在 Arduino IDE 中工作。也就是说，如果 Arduino 有任何负面的属性，那就是 IDE。很简单，没有调试器。

实力来源于平台的标准化。你可以将 Arduino 标准适配到你制作的电路板上，这种适配应该允许 Arduino 的无数库与你的新硬件一起工作。这是生态系统的强大优势。与此同时，这种简单的启动和运行方式也导致了许多之前讨论过的负面联想。

所以你有它。Arduino 与任何其他微控制器没有什么不同，完全可以用于消费类产品中，例如手机、武器等。不这样说是愚蠢的。

## 消费产品中 Arduino 的优点是什么？

这是*问黑客日*，这样你就知道有一个问题正在酝酿中。消费产品中 Arduino 的优点是什么？如今，大多数电子产品都有设备固件升级(DFU)模式，允许最终用户升级代码，因此 Arduino 在这方面没有优势。有人可能会说，使用 Arduino 意味着代码是开源的，因此社区改进的时机已经成熟，但闭源二进制文件仍然可以在平台上分发。然而，有许多产品已经成功地打开了来自发布代码和邀请改进的“社区倍增器”。

你认为围绕 Arduino 构建消费品的好处是什么，未来会是什么样子，我们将如何实现？在下面留下你的想法！