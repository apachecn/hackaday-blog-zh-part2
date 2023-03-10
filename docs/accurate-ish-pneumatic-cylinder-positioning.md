# 气缸定位相当精确

> 原文：<https://hackaday.com/2013/10/20/accurate-ish-pneumatic-cylinder-positioning/>

![pneumatic flow positioning](img/f9090c24514132f336ab5d8166ca2d01.png)

气压缸定位？如果你有技术背景，你现在应该正在挠头。气压缸定位？那真不应该起作用！嗯，[arduinoversusevil]已经黑进了一个系统，这个系统…[有点像是在工作](http://arduinoforgoodnotevil.blogspot.de/2013/10/accurate-ish-pneumatic-cylinder.html)。

首先介绍一下[arduinoversusevil]的背景。他正在制造一个液压/气动调酒机器人。太棒了。

不管怎样，他最近以近乎零的价格买了一个旧液压缸，并决定试着摆弄它。他清除了里面的油，现在正把它用作气压缸。他还买了一个 10 美元的廉价塑料 Adafruit 流量计，并决定尝试制作一个定位气压缸。他使用 Launchpad 开发板，通过危险的原型 ATX 分线板控制电磁阀。令人惊讶的是，廉价的 Adafruit 流量计足够精确，足以测量气缸中的空气量，根据负载，可以使用该流量计来稍微精确地定位气缸。

在流量计损坏之前，他进行了大约 360 次循环的测试，并且能够达到大约 5 毫米的精度！一点也不差。休息后留下来看看它的运行——听听他丰富多彩的评论。

[https://www.youtube.com/embed/Gmt7iVCwDKY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Gmt7iVCwDKY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [危险原型](http://dangerousprototypes.com/2013/10/18/accurate-ish-pneumatic-cylinder-positioning-with-flow-meter-atx-breakout-and-msp430-launchpad/)