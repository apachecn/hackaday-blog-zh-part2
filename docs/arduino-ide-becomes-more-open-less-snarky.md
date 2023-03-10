# Arduino IDE 变得更加开放，不那么刻薄

> 原文：<https://hackaday.com/2015/05/13/arduino-ide-becomes-more-open-less-snarky/>

Arduino IDE 的 1.6.4 版本已经发布了一段时间，它有一些显著的变化。在我们看来，最有趣的变化是在 Arduino IDE 中增加对非标准板及其配置的支持变得更加简单。我们将在下面详细讨论。

但在此之前，是时候告别厚脸皮的小弹出窗口了，当使用带有前合作伙伴变成竞争对手的 USB IDs 的主板时，它会发出警告信息。我们绝对[同意【马西莫】](http://blog.arduino.cc/2015/04/28/opening-up-the-arduino-ide/)的观点，Arduino SRL / Smart Projects 和 Arduino LLC 之间的[问题在社区中已经](http://wp.me/pk3lN-CRf)[众所周知](http://wp.me/pk3lN-Dk3)，现在是弹出窗口消失的时候了。

现在谈谈这篇文章的核心内容。新的“板管理器”功能使其他非 Arduino 产品在 Arduino IDE 中编程变得更加容易。Adafruit 有一个关于在他们的产品中使用电路板管理器功能的[教程](https://learn.adafruit.com/add-boards-arduino-v164?view=all)，它基本上可以归结为“输入正确的 URL，点击你想要的电路板，下载，重启 Arduino，砰！”

非官方支持的第三方董事会名单仍然有点短，但它包括了一些明星条目。例如，Adafruit 提供了 ESP8266 所需的文件，该文件最近接受了 Arduino 处理。这意味着您可以简单地将您的 IDE 指向 Adafruit 的 URL，它将从舒适的 Arduino IDE 中为您设置为 ESP8266 开发所需的一切。

从我们的角度来看，另一个突出之处是这个链接[简化了 Arduino IDE 对裸 AVR 芯片](https://raw.githubusercontent.com/carlosefr/atmega/master/package_carlosefr_atmega_index.json)的编程。虽然将 Arduino 代码编程到简单的 AVR ATmega168 中一直是可能的，但从来没有像现在这样容易。

## 它是如何工作的

在引擎盖下，新的董事会经理制度相当简单。点击其中的一个链接，就会看到一个 JSON 文件，其中包含任意数量的电路板架构定义。每个条目都提供了用于在 Arduino IDE 的下拉菜单中生成菜单项的目标板的文本描述，以及指向 zip 文件的链接。这个 zip 文件包含了使 Arduino 库适应目标电路板或芯片所需的一切。

例如，像 bare-AVR 修改这样简单的事情，zip 文件只包括 boards.txt 和 platform.txt 文件，Arduino IDE 使用它们来填充许多特定于电路板的参数，如 CPU 时钟速度、熔丝位设置和用于刷新新代码的 AVRDUDE 命令选项。对于更复杂的事情，如将 Arduino 移植到 ESP8266，zip 文件还包括移植的 Arduino 核心和库函数，以及使 Arduino 在该目标上工作的上传工具。

对第三方设备如此透明地开放 Arduino IDE 是一个非常有趣的实验。它肯定会赢得黑客和*duinos 零售商的青睐，我们猜测它只会鼓励将 Arduino 库移植到更多的平台上。让我们看看这个社区将如何发展。接下来你想看到 Arduino 移植到什么？