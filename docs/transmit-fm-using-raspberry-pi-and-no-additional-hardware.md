# 使用 Raspberry Pi 传输 FM，无需额外硬件

> 原文：<https://hackaday.com/2012/12/10/transmit-fm-using-raspberry-pi-and-no-additional-hardware/>

现在这里有一个项目，它实际上破解了 Rapsberry Pi，而不仅仅是将其用作嵌入式计算机。[伦敦探险家]想出了如何把 RPi 变成一个调频发射机。目前，它完全是在用户空间中完成的，但我们确信，如果有人想进一步深入硬件，它可以得到改进。对于那些想尝试一下的人来说，他已经将所有东西都打包到一个简单的 python 包中。

这项技术不需要任何额外的东西，只需要一根 20 厘米长的电线作为天线。诀窍是将 GPIO 引脚 4 映射到内存中的一个位置。然后使用时钟发生器将此引脚切换到 100 MHz，这是您的无线电应该调谐到的频率。分数分频器根据传输的声音文件调整频率。

这一概念的证明能够在大约 50 米的距离内穿过几堵墙进行可靠的传输。问题是这种技术在可发送的数据量上受到限制。目前只有大约 6 位音频。但是深入抽象层使用 DMA(直接内存访问)可能会有所改进。

[感谢欧文通过 [Reddit](http://www.reddit.com/r/raspberry_pi/comments/14k5o3/raspberry_pi_fm_transmitter_with_no_additional/)