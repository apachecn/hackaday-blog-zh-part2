# 拿起一枚 NeoPixel 戒指，看看你能用这个教程做些什么

> 原文：<https://hackaday.com/2014/07/21/pic-up-a-neopixel-ring-and-c-what-you-can-do-using-this-tutorial/>

![lit ring](img/224fa3e607b582525bef222e72bb7443.png)正如【Shahriar】在他的最新视频【T2 在信号路径】的介绍材料中指出的，Arduinos 是初学者挖掘各种电子兴奋的好方法，但他们这样做的代价是将初学者与微控制器的细节隔离开来。在这里，[Shahriar]从单个 RGB LED 的勇气和荣耀开始，给出了一个 60-neopixel 戒指的非常彻底的演练。然后，他展示了如何使用 PIC 和一些 c 语言轻松地对戒指进行编程。

[Shahriar]的评估板是一个简单的设置，他用于其他项目。这是基于 PIC18F4550，他用 ICD U64 编程。PIC 通过 USB 供电，但他使用一个单独的开关电源为戒指本身供电，因为他需要每 RGB 约 60mA 的电流才能使它们以最大亮度发出白光。

他编写了一个简单的头文件，该文件引入了 18F4550 库，设置了保险丝，并定义了一些特定于戒指尺寸的常数。正如他在视频中解释的那样，PIC 可以从一个 20Mhz 的晶体创建一个 48MHz 的内部时钟，他还在报头中设置了这种延迟。主要代码处理波形生成，而[Shahriar]很好地解释了如何用单个引脚来处理这个问题。在点亮环之前，他将示波器放在分配的 GPIO 引脚上，以表明尽管数据手册中关于 0 位低电平周期的未延迟宽度是错误的，但它仍然可以对 led 进行编程。

[Shahriar]在他的网站上有代码。他还向美国居民提供赠品:只需在他的博客帖子或 YouTube 上的视频上发表评论，你就可以赢得一台带探头和手册的 [TPI Scope Plus 440](http://www.kiesub.com/prostores/servlet/-strse-385/TPI-440-Scope-Plus/Detail) 或一台带 GPIB 的[泰克 TDS2232](https://www.youtube.com/watch?v=h8MamgRaLsM) 。他甚至会付运费。

[https://www.youtube.com/embed/EXr2_zSfnFw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EXr2_zSfnFw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)