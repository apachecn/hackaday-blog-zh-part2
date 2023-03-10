# ESP8266 作为网络 MP3 解码器

> 原文：<https://hackaday.com/2015/06/06/esp8266-as-a-networked-mp3-decoder/>

支持库、优秀的应用笔记和来自制造商的工作示例确实有助于我们用新器件制造酷炫产品。Espressif Systems 公司的 ESP8266 产品一直做得很好(当然，这不会损害低于 5 美元的 IOT 设备成为现实)。然而，直到最近，他们才开始发布完整、复杂的应用程序示例。这个演示，一个联网的 MP3 网络收音机播放器，刚刚出现在 Github 上，作者是我们更熟悉的人 [Sprite_tm](http://spritesmods.com/) 。我们迫不及待地想看到更多。

MP3 解码器本身是 [MAD MP3 库](http://www.underbit.com/products/mad/)的一个端口，适用于较小数量的 SRAM，并移植到 ESP8266。例如，通过几个外部部件，你可以制作一个连接互联网的设备，你可以指向任何 Icecast MP3 流，它会解码并播放产生的音频。

你会问，什么外部零件？首先是做数模转换。正如所写的那样，该应用程序是为 ES9023 DAC 构建的，但基本上，只要稍微浏览一下数据手册，抓抓脑袋，任何说 I2S 的东西都应该是可行的。当然，您可以去掉听起来不错的 DAC 芯片，直接从 ESP8266 输出 5 位 PWM，但除了是一个不错的快速演示之外，它听起来就像废话。

另一个建议的外部 IC 是 SPI RAM 芯片，可以缓冲输入的 MP3 文件。WiFi——以及一般的 TCP 网络——是什么，你会想要缓冲 MP3 文件，以防止故障。与专用 DAC 一样，没有它也可以(在“playerconfig.h”文件中有这样做的定义),但你可能会后悔。

总之，一个 ESP8266 芯片，一个便宜的 I2S DAC，和一些外部 RAM，你就有了一个 webradio 播放器。好的，也许我们还会增加一个放大器芯片、电源和一个扬声器。嗯嗯……还有显示器？还是通过 WiFi 进行配置？重点是，这是一个很好的工作代码示例，也是一个整洁的 DIY 设备，可以向您的朋友展示。

缺点是什么？到目前为止，只有单声道版本的 libMAD 解码器/合成器被移植到 ESP8266 上。github 链接正在请求一个 pull 请求，未导入的代码就在那里，我们认为应该有人承担这个任务。

## 其他资源

在我们搜索 ESP8266 的其他代码示例时，我们偶然发现了三个似乎是 Github 上的官方 Espressif 知识库: [espressif](https://github.com/espressif?tab=repositories) 、 [EspressifSystems](https://github.com/EspressifSystems?tab=repositories) 和 [EspressifApp](https://github.com/EspressifApp?tab=repositories) (用于连接到 ESP8266 的移动应用)。官方的“[低功耗电压测量”示例](https://github.com/EspressifSystems/low_power_voltage_measurement)看起来是一个很好的起点，它使用了当前版本的 SDK 和工具链。

还有一个[活动论坛](http://bbs.espressif.com/)，有他们自己的[社区 Github 库](https://github.com/esp8266)，有几个[【你好世界】的例子](https://github.com/esp8266/source-code-examples)和[一个很好的工具链演练](https://github.com/esp8266/esp8266-wiki/wiki/Toolchain)。

当然，我们过去也报道过一些。例如，这个应用程序跟踪电池电量。如果你有时间，看看[Hackaday](http://hackaday.com/tag/esp8266/)上所有标记为 ESP8266 的帖子。

您不可能需要更多资源来开始您的 ESP8266 项目。哦，等等，你想要 Arduino IDE 支持？

感谢[Sprite_tm]的提示。