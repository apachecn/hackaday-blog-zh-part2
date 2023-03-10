# Arduino 的 GPU

> 原文：<https://hackaday.com/2013/10/15/a-gpu-for-an-arduino/>

![GPU](img/9755ad996c3a48094d81f0a2f830acba.png)

作为 Gameduino 的创造者，一个为任何 Arduino 添加 VGA 端口和图形功能的屏蔽，[James]知道一些关于用微控制器生成高质量视频的知识。他的最新作品《Gameduino 2》让他之前的作品相形见绌。他创造了一个内置触摸屏的 Arduino shield，其图形性能与 20 世纪 90 年代末的 Quake box 相同。

这个盾牌背后的动力来自一个名为 [FTDI EVE](http://www.ftdichip.com/EVE.htm) 的单芯片图形解决方案。这不是[我们第一次听说 FTDI EVE](http://hackaday.com/2013/03/01/cool-new-hardware-spectacular/) ，但这是第一个使用这个非常酷的嵌入式图形引擎的项目或产品。Gameduino 2 通过 SPI 连接使用 FT800 图形芯片，为 480×272 TFT 触摸屏提供与 Voodoo 2 显卡相同的图形功能。从视频来看，[詹姆斯]能够在一个屏幕上显示成千上万个精灵，以及简单的 3D 动画，并且只用一台 Arduino 就能显示出令人印象深刻的 2D 动画。

虽然 Gameduino 2 被设计成一个你自己编程的游戏控制台，但我们认为它作为独立项目的显示器会更加有用。