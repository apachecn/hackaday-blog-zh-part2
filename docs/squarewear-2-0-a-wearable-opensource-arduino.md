# SquareWear 2.0 A 可穿戴开源 Arduino

> 原文：<https://hackaday.com/2014/01/12/squarewear-2-0-a-wearable-opensource-arduino/>

![squarewear2_annotation-1024x577](img/829a3181b076e3ba3a29c62488a828e0.png)

你们厌倦了重新设计的 Arduinos 了吗？通常我们是这样，但是[Ray]刚刚发布了 [SquareWear 2.0](https://rayshobby.net/?p=7964) ，我们不得不承认，这是一个非常巧妙的设计。

这是我们一年前报道过的 SquareWear 1.1 [的更新。这个版本使用了 18F14K50 微控制器，尺寸只有 1.6 英寸 x 1.6 英寸，可以很容易地缝进可穿戴的电路中。但是在收到许多设计基于 Arduino 的新主板的请求后，[Ray]欣然同意并开发了 v2.0](http://hackaday.com/2012/11/15/squarewear-sewable-microcontroller-board/)

新的 SquareWear 略大，尺寸为 1.7 英寸 x 1.7 英寸，但它的冲击力更大，功能更强——看看上面的示意图就知道了！唯一的问题是它实际上没有 USB 转串行芯片，这就是为什么[Ray]能够让电路板如此小而便宜。相反，它使用 [V-USB](http://www.obdev.at/products/vusb/index.html) 库在软件中模拟 USB。这种方法要慢得多，但仍然有效。为了通过 USB 端口执行串行通信，它使用板载 USBasp 引导加载程序。

该板还具有大的通孔，以容纳可缝合的引脚垫，使其非常容易集成到织物中！

关于 SquareWear 2.0 的完整解释，请查看休息后的视频。

[https://www.youtube.com/embed/sCp4sILWcoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sCp4sILWcoc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)