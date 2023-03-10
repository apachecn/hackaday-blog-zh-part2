# TDOA(到达时间差)定向天线

> 原文：<https://hackaday.com/2014/03/04/tdoa-time-difference-of-arrival-directional-antenna/>

![tdoa-antenna-tutorial](img/8d54bbf69c06b129259c2e72f9589ccf.png)

我们过去曾发表过关于定向天线的文章，比如用于发射机搜索的八木天线。这些类型的天线和接收都有一个主要缺点，那就是当你靠近发射机时，S 表会满量程。此时发射的信号似乎来自所有方向。为了纠正这个问题，你需要使用巧妙的信号衰减器，或者换一个质量差的接收天线，同时有效地关闭频率，使你的接收机难以听到，这样只有直接通往发射机的路径才是最响的。

还有一种流行的天线，你可以自己制作，叫做 TDOA，代表到达时间差。[Byon Garrabrant N6BG]分享了一个简短的视频[教程，介绍了他自制的 TDOA 天线](http://www.youtube.com/watch?v=JVGf28ckHyg)的功能。实际上，这是一个有源天线，使用 555 芯片，或者在[Byon 的]情况下，使用 PIC 芯片，在缩短码尺两端的两个接收偶极天线之间快速切换。在他的解释中，你了解到随着天线末端靠近或远离声源，随着天线与声源的距离变得相等，产生的 640 Hz 音频音调将从响亮变得非常柔和。这种定向接收不受信号强度的影响。这意味着你可以非常接近一个强大的发射机，它仍将作为一个良好的定向天线。

当前的电路图、BOM 和源代码都可以在[【Byon’s】TDOA 页面](http://byonics.com/tdoa/)上找到。

[Byon]在他的设计中使用可编程 PIC 而不是 555 的原因是因为他想增加一些修改，例如将音频输出反馈到 PIC，以便通过编程打开指示发射机方向的左侧或右侧 LED。此外，他计划在三角形配置中添加第三个天线，以编程方式控制一圈 6 个 led，指示信号的确切方向。当他完成最后的修改后，他可以带着他车上的天线阵列和里面的发光二极管圆圈来指示准确的导航方向。

我们期待着看到其余的发展，甚至有一天可能成为一个工具包。休息过后，你可以观看(Byon 的)TDOA 视频。

[https://www.youtube.com/embed/JVGf28ckHyg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JVGf28ckHyg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)