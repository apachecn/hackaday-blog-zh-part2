# 深入研究 APA102 串行 LED 协议

> 原文：<https://hackaday.com/2014/12/09/digging-into-the-apa102-serial-led-protocol/>

[Tim]得到了一些 APA102 RGB LEDs，其功能类似于我们在许多项目中看到的常见 WS2812 可寻址 led。APA102 LEDs 的优势在于它们没有 WS2812 的严格时序要求。这些 led 由 SPI 总线控制，SPI 总线可以以任意速率计时，因此可以轻松用于几乎任何微控制器或嵌入式系统。

在使用 led 后，[Tim]发现 led 的功能与数据表中的功能有所不同，这让他相信了。[Tim]用 ATtiny85 控制了一串 APA102 LEDs，并在一些 led 之间连接了逻辑分析仪。他发现 SPI 接口的时钟信号不只是通过每个 LED，它实际上看起来像是在输出端反转了。经过一些调查，[Tim]发现时钟信号在传递到下一个 LED 之前会延迟半个周期(看起来像反转)。这为链中的下一个 LED 提供了足够的时间，使数据线上的数据在锁存之前变得有效。

由于时钟被延迟，[Tim]发现必须将额外的位作为“结束帧”计时，以生成时钟信号，将剩余的数据传播到链的末端。虽然数据手册规定了 32 位端帧，但这只适用于最多 64 个 led 的串。对于更长的线，端架必须增加更多位，数据手册甚至没有提到这一点。查看[Tim]的帖子了解更多信息，他将带您了解他对 APA102 LEDs 的逻辑分析。