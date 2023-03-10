# 喜怒无常的无用机器

> 原文：<https://hackaday.com/2013/12/20/moody-useless-machine/>

如果你厌倦了在网上寻找下一个大项目的灵感，试试在 YouTube 上搜索“无用的机器”。在看了几个小时这些毫无意义但又很搞笑的作品后，我们确信你会想要做一个。对我们来说幸运的是，[Arvid]记录了他的[穆迪无用机器](http://www.lamja.com/?p=451)的设计，让你开始。

为什么【阿维德的】机器喜怒无常？好吧，为了充分理解一台无用机器的情感敏感性，你首先需要理解它们做什么和不做什么。这里只需要一句话的解释；你扳动一个开关，机器就把开关扳回来……就是这样。[Arvid]用一个独立的 Arduino 实现了一个双伺服系统，这使他能够给他的机器赋予“个性”。有时，开关会毫无争议地迅速退回，有时，机器会大发脾气。

虽然这台机器毫无用处，但里面的电子设备一点也不差。为了保持一切整洁和无害，机器由电池供电，因此[Arvid]将 Arduino 置于“睡眠”模式，直到开关被拨动。该开关被配置为 Arduino 上的中断，切换时会唤醒 Arduino。一旦 Arduino 被唤醒，它通过功率 MOSFET 给伺服系统供电，然后一切准备就绪；机器做出响应并回到“睡眠”状态。这是一个伟大的项目，但信不信由你，事情会变得更加无用，就像这台[先进的无用机器。](http://hackaday.com/2012/12/22/an-even-more-useless-machine/#more-92186)

[https://www.youtube.com/embed/-PqcCjFaf3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-PqcCjFaf3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [被黑的小工具](http://hackedgadgets.com/2013/12/19/microcontroller-based-useless-machine/)