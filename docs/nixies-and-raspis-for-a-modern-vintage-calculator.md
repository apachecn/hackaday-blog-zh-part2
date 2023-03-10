# 现代老式计算器的 Nixies 和 Raspis

> 原文：<https://hackaday.com/2014/11/06/nixies-and-raspis-for-a-modern-vintage-calculator/>

有一些非常罕见和非常昂贵的带有数码管显示器的计算器散布在计算器的历史中，但到目前为止，我们还没有看到有人从零开始建造一个真正有用的谢妮计算器。[【斯科特】就是这么做的](http://www.smbaker.com/wordpress/wp-content/uploads/2014/11/nixiecalc_keyboards_1024.jpg)。这是一个完整的、全功能的电子计算器，具有标准科学计算器的所有功能。

该计算器使用 IN-12 Nixies，这是任何想要制作时钟或其他数字氖放电显示器的人的标准。每个谢妮由 K155D 驱动芯片控制，驱动芯片由 I2C IO 扩展器控制。

键盘是这变得有趣的地方；电子是一回事，但机电和按钮是令人头痛的全新来源。[Scott]最终使用了 Cherry MX Blue 开关，这是机械键盘更常见的开关之一。通过使用标准的键盘开关，[Scott]能够为他的计算器上的每个按钮定制键帽。

计算器的大脑是一个树莓派，I2C 引脚会关闭以监听设备上的几个 IO 扩展器。一个 Raspi 可能有点大材小用，但一个联网的计算器确实允许[Scott]将计算结果发送到 WolframAlpha，甚至是每个 pi 中都包含的 Mathematica 副本。

[Scott] [已经把他的项目放到了 Kickstarter](https://www.kickstarter.com/projects/1555102420/nixie-tube-calculator) 上。下面的视频。

[https://www.youtube.com/embed/5f17FyCIR-U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5f17FyCIR-U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/LM06CDzEpKk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LM06CDzEpKk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/pt0YVQzNv0Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pt0YVQzNv0Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)