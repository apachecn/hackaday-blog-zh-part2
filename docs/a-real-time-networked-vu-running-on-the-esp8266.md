# 在 ESP8266 上运行的实时网络 VU

> 原文：<https://hackaday.com/2015/02/17/a-real-time-networked-vu-running-on-the-esp8266/>

尽管 ESP8266 WiFi 芯片组非常便宜(并且使用起来有些困难)，但它们仍然具有很强的处理能力。例如，[Mr.jb.swe]采用其中一个模块，制作了一个带 WS2812B LED 灯条的[独立实时 VU 测量仪](http://hackaday.io/project/4318-vu-meter-esp8266-ws2812b)。VU 完全在 ESP 芯片上运行，不需要任何额外的微控制器。这是一个例子，我们认为许多项目可以效仿，以消除未使用的马力(额外的微控制器)，有时用于避免直接在 ESP 上编程。你可以用这些模块做的东西是野生的…你看到这个 [WiFi 信号强度映射项目](http://hackaday.com/2015/02/17/mapping-wifi-signals-in-3-dimensions/)了吗？

ESP 芯片组充当 UDP 客户端，从[Mr.jb.swe]编写的 WinAmp 插件接收数据包。该插件不断计算正在播放的任何曲目的 dB，并通过 WiFi 将其传输到他的 ESP8266。他还提到 ESP 芯片组的 ADC 也可以用于音频采样，尽管这几乎消除了对 WiFi 的需求。

即使处理器正在解析 UDP 消息、驱动 WS2812 条、驱动小型有机发光二极管显示器进行调试，整个设置的响应速度也非常快，而且它甚至没有使用单独的微控制器。[JB . SWE 先生]还发布了他的代码片段，让你开始自己的项目。休息之后，请观看视频，了解实际情况。

[https://www.youtube.com/embed/5O1pW-jE2d0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5O1pW-jE2d0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/leA747pM-jw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/leA747pM-jw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)