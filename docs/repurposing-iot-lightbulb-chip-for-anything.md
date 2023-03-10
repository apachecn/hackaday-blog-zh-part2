# 改变 IOT 灯泡芯片的用途

> 原文：<https://hackaday.com/2015/02/15/repurposing-iot-lightbulb-chip-for-anything/>

家庭自动化产品在消费主义的世界里达到了临界质量，现在突然每个人都有一个你可以使用某种协议控制的产品。Cree(led 的制造商)有一种相当便宜的 IOT 灯泡，在加拿大和美国以 15 美元的低价出售——考虑到普通的 LED 灯泡可以在没有无线连接的情况下运行那么长时间，这还不错！

所以，如果你想给你的房子装上智能灯，那太好了。但是其他的事情呢？嗯，[Mac Alpine]决定砸开其中一个灯泡，看看他能否重新利用 IOT 板。事实证明，你可以。

事实上这几乎太方便了。这是一个非常小的芯片，大约只有一枚银元的一半大小。它有一个小的 ZigBee 无线电模块。你只需要一个 3V 电源，然后嘣——你就有了一个能够输出 PWM 的 IOT 模块。它具有一个 Atmel ATSAMR21E 微处理器，通过无线电与一个古怪的 Wink hub 通信，也可以使用 IFTTT 触发。

[https://www.youtube.com/embed/SE-yrFMJDXo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SE-yrFMJDXo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

你可以更深入地研究这一技术，为它编写自己的控件——或者，你可以利用已经可用的应用程序——但不管怎样，这可能是为你的家庭添加一些可靠的智能控件的一种非常廉价的方式。或者你可以什么都不做。