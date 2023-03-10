# 迎接新年的亮闪闪的软呢帽

> 原文：<https://hackaday.com/2013/01/08/a-blinky-fedora-to-ring-in-the-new-year/>

[加勒特·梅斯]决定在新年前夜穿得喜庆些。他想出的是一顶环绕着发光二极管的软呢帽，能对音乐做出反应。硬件使用条带上的 5050 个 led。它们中的三个环绕着头部装置，总共提供 114 个 RGB 像素。每一个都是 WS2811 模块— [一个我们最近越来越多地看到的部分](http://hackaday.com/2013/01/02/three-conceptual-approaches-to-driving-a-ws2811-led-pixel/)。

休息后的视频剪辑以几分钟的演示开始。[Garrett]设法为硬件编写了各种动画，包括几种不同风格的颜色扫描和淡入淡出。你可能会开始认为这三个波段总是显示相同的模式，但继续观察，你会看到一个火花模式，证明每个点可以单独处理。

视频进行到大约 2:20 秒时，[Garrett]解释了他是如何完成的，并展示了驱动程序硬件。这些带子粘在帽子上滑动的带子上。驱动灯的电线穿过一些降落伞的中心，并连接到 3D 打印外壳中的 Arduino。电源由带 ShiftBrite 屏蔽的便携式 USB 电池提供，MSGEQ7 芯片完成零件列表。

[https://www.youtube.com/embed/cGoYTl2KF4c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cGoYTl2KF4c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/electronics/comments/162xw6/114_rgb_led_soundreactive_fedora_for_new_years/)