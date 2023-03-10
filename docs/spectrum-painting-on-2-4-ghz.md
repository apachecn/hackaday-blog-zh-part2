# 2.4 GHz 上的频谱绘画

> 原文：<https://hackaday.com/2015/08/22/spectrum-painting-on-2-4-ghz/>

给几千名极客一个软件定义无线电(SDR)平台，可以预见会发生什么:黑客必须攻击。我们只是惊讶这一切发生得这么快。 [Spectrum Painter](https://github.com/polygon/spectrum_painter) 是第一批从[2015](http://hackaday.com/tag/cccamp/)CCCamp 颁发的 rad1o 徽章中脱颖而出的酷炫黑客之一。这使得在几个不同的 SDR 硬件平台上以 [Hellschreiber](https://en.wikipedia.org/wiki/Hellschreiber) 模式发送图像变得非常简单。

我们特别喜欢这个项目的简单之处。不要误解我们，我们是 GNURadio 和 T2 GNURadio 伙伴软件无线电黑客环境的超级粉丝。但是如果你只是想做一些简单的事情，比如发送一张笑脸的图片，那么功能齐全的 GNURadio 套件就有些过头了。

[HackRF](http://greatscottgadgets.com/hackrf/) 、 [rad10 badge](http://hackaday.com/2015/07/12/cccamp-2015-rad1o-badge/) 、 [bladeRF](http://hackaday.com/2013/02/02/bladerf-your-next-software-defined-radio/) 都有软件可以让你直接通过无线电接口加载并播放文件；它就像一个 WAV 文件，只是在无线电频率。这使得像 Spectrum Painter 这样的黑客变得非常简单。只需将图像文件转换成相应的无线电波形数据，然后发送出去。没有图形用户界面，没有拖动，没有放下。

```

img2iqstream -s 1000000 -l 0.004 -o smiley.iqhackrf --format hackrf examples/smiley.png
hackrf_transfer -t smiley.iqhackrf -f 2450000000 -b 1750000 -s 1000000 -x 20 -a 1

```

嘭！kudos[多边形]！

如果所有这些特别提款权的行动激起了你的兴趣，有[很多事情你可以做](http://hackaday.com/?s=rtl-sdr)甚至只是用一个 El cheapo RTL-SDRu 盘接收。这是进入 SDR 的入门药物，所以如果你还没有上瘾，而且你有一个空闲的周末，试试吧。