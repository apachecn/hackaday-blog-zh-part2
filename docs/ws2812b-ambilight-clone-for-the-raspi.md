# 用于 Raspi 的 WS2812b 流光溢彩克隆

> 原文：<https://hackaday.com/2014/03/26/ws2812b-ambilight-clone-for-the-raspi/>

对于 Raspberry Pi 被用作媒体服务器的频率，以及将一束 led 连接到 Pi 上的 GPIO 引脚是多么容易，我们很惊讶我们以前没有见过类似 Hyperion 的东西。它使用非常常见的 WS2812b 独立可控 RGB LEDs，以屏幕边缘的颜色环绕电视后面的墙壁。

Hyperion 的一大特点是它能够控制大量的发光二极管；一个 50 个 LED 灯只消耗了 Pi 的 1.5%的 CPU。它通过在 2MHz 下运行的 Pi 上实现的“迷你 UART”来实现这一点。

只有一个额外的组件需要运行一个巨大的带 Pi 的 RGB LEDs 灯——一个用 HCT 系列逻辑芯片制成的某种反相器。之后，你只需要连接电源，就可以在电视或显示器后面享受炫目的显示。

谢谢[emuboy]送来这个。