# 廉价的 AVR 编程器由五个组件组成

> 原文：<https://hackaday.com/2014/11/02/inexpensive-avr-programmer-made-from-five-components/>

如果你想以尽可能低的成本编写 AVR 芯片，那么[Ian 的]解决方案可能正适合你。他只用四个组件就造出了一个 AVR 编程器。该设计基于 [vusbtiny](http://www.simpleavr.com/avr/vusbtiny "vusbtiny") AVR 编程器设计，省略了一些组件。

[Ian 的]设计省去了两个电阻和两个二极管，只剩下四个元件。其中包括一个 1.5k 电阻、一个小电容、一个 USB 连接器、一个六引脚接头和一个 ATtiny45。他承认这可能不完全符合 USB 规范，但它确实有效。

这是其中一个项目，它实际上是一个“它会工作吗？”比什么都重要。事实上，你需要首先对 AVR 芯片进行编程，这意味着这在紧要关头没有用，因为你已经有一个工作的程序员了。尽管如此，看到用尽可能少的资源能做些什么总是很有趣的。