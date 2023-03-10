# 另一个采取后窗 LED 字幕

> 原文：<https://hackaday.com/2013/01/09/another-take-on-the-rear-window-led-marquee/>

![re-window-led-display](img/6da898cff5282765ca62d5e7083eb3f6.png)

这个[后窗 LED 罩](http://dunnrightsoftware.com/arduino/)将有助于让你后面的司机知道你何时计划变道或转弯。但是它也包括发送类似“后退！”的信息的能力。[罗伯特·邓恩]在看到我们在 10 月份报道的[后，受到启发，开始着手这个项目。我们会说，他的有一个更好的机会成为街头合法，因为它使用所有的红色发光二极管。](http://hackaday.com/2011/10/20/rear-window-led-display-gives-other-drivers-a-piece-of-your-mind/)

这个跑马灯是由 480 个 led 组成的矩阵，全部手工焊接成几乎透明的 48×10 网格，如上图所示。这对保持他卡车后窗的视野很重要。这让我们怀疑用 SMD 代替通孔元件的可行性。这肯定会使它在没有照明的情况下更加不可见，但组装过程会更加困难。这是因为 5 毫米的 LED 封装非常适合他在一些胶合板上钻的孔，这些孔在焊接过程中用作夹具。引线的存在也使得焊接过程易于管理。

Arduino 板的电源由点烟器适配器提供。一组六个移位寄存器驱动列，而行由 4017 十进制计数器和一些晶体管控制。休息后查看 blinker 测试视频，看看它在路上能做什么。

[https://www.youtube.com/embed/oAguppeRYMQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oAguppeRYMQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)