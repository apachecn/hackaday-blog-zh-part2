# Arduino 驱动的警报系统拥有所有的铃铛和哨子

> 原文：<https://hackaday.com/2014/09/02/arduino-powered-alarm-system-has-all-the-bells-and-whistles/>

抛开所有使用 Arduino 来闪烁几个 led 或驱动一个伺服电机的项目。[IngGaro]的最新项目使用了这种多功能微控制器的全部功能，并将 Arduino Mega 变成了一个功能齐全的家庭报警系统。

报警器可以读取 RFID 卡来激活和控制设备。它通过 I2C 总线与前面板通信，并且可以控制窗户或百叶窗的打开和关闭。还有一个集成的 GSM 天线，用于通过蜂窝网络传达任何紧急情况。该设备还能跟踪温度和湿度。

整个系统可以通过网络界面进行控制。Arduino 提供了一个网页，允许用户完全控制警报。有了所有这些，很难想出这个微型微控制器还有什么功能，除非你想增加一个[该死的激光器](http://hackaday.com/2010/01/03/arduino-security-with-frickin-laser/)来真正绊倒窃贼！