# 800 英寸每分钟，分辨率为 0.00025 英寸

> 原文：<https://hackaday.com/2014/08/28/800-inches-per-minute-at-0-00025-resolution/>

PONTECH 的人刚刚发布了一个令人印象深刻的开源 PIC32 库，用于控制速度为每分钟 800 英寸的线性滑轨！

PONTECH 制造基于开源芯片套件平台的 Quick240(快速通用工业控制卡)。它是为工业自动化系统设计的，在这些系统中通常会使用梯形逻辑 PLC。使用这样一个系统的好处是，因为它是开放的，你不再被专有的硬件所束缚，它可以更加灵活地允许你“做你自己的事情”。我们提到过它也兼容 Arduino 吗？

使用这个系统，他们成功地控制了两个 8 英寸的 Velox 幻灯片，速度高达每分钟 800 英寸，分辨率为 0.00025 英寸——只需看看下面的视频，就能体会到这有多快。

[https://www.youtube.com/embed/f44oHby9aMw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/f44oHby9aMw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

StepAndDirection 库可在 [GitHub](https://github.com/pontech/pic32lib) 找到，用于 PIC32 微控制器。