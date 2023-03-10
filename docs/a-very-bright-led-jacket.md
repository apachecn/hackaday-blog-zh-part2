# 一件非常亮的 LED 夹克

> 原文：<https://hackaday.com/2014/09/26/a-very-bright-led-jacket/>

去年【Ytai】第一次去火男。他有点缺乏经验，缺乏让他出现在舞台上的流明。今年，他制作了一个额外的[明亮的 LED 夹克](http://ytai-mer.blogspot.ca/2014/09/fairydust.html)来弥补这个缺陷。

该外套由 48 个 led 组成，每个 150 流明。每个 RGB LED 模块都放置在自己的 PCB 上，由微型 [PIC12F1571](http://www.microchip.com/wwwproducts/Devices.aspx?product=PIC12F1571) 微控制器控制。这个微控制器非常适合，因为它有三个 PWM 通道(每种颜色一个)，价格为 50 美分。PIC 上的固件允许电路板以菊花链形式连接在一起，以减少布线。这是通过使用类似于流行的 WS2811 LEDs 的协议来实现的。

组装 50 块电路板是一项挑战。这个问题是通过使用表面贴装元件、来自 [OSH Stencils](http://www.oshstencils.com/) 的焊料模板、电锅和足够的耐心解决的。每个模块的最终成本约为 3 美元。

将 50 块木板拼在一起，就缝制出了一件双层夹克。电子产品被夹在这两层织物之间，这使得夹克看起来很干净。安装在手腕上的控制器允许佩戴者选择不同的模式。

要想全面了解这件夹克，请在休息后观看视频。

[https://www.youtube.com/embed/W0b854OpM2U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/W0b854OpM2U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)