# 在廉价的 GPS 上寻找有效的 TX 引脚

> 原文：<https://hackaday.com/2015/01/30/finding-an-active-tx-pin-on-cheap-gps/>

20 欧元将为你赢得一个小型的独立 GPS 钥匙链。打开箱子，你会得到更多。[j3tstream]探索了这个东西的内部，发现 [NMEA 数据可以从 GPS 芯片](http://www.weirdlab.fr/?p=510)的 TX 引脚流出。

首先，看看那个微型 GPS 天线模块，太疯狂了！但是我们跑题了。出于测试目的，探测了 GPS 的异步 UART，证明可以获取数据。从那里[j3tstream]移动到一个带有 SD 卡的 Arduino Pro Mini，用于数据记录。uC 由 GPS 板供电，但这会很快耗尽电池，所以[j3tstream]用旧手机换了一个。

该设备附带的小点阵液晶显示器也引起了我们的注意。如果你能为 GPS 黑一个无头接口，它可以被重新用于你的下一个项目。我们可以为它建议一个可穿戴游戏项目吗？