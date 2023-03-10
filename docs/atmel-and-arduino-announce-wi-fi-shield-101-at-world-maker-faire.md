# Atmel 和 Arduino 在世界创客大会上发布 Wi-Fi Shield 101

> 原文：<https://hackaday.com/2014/09/30/atmel-and-arduino-announce-wi-fi-shield-101-at-world-maker-faire/>

[https://www.youtube.com/embed/IjxFQkW2uUM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IjxFQkW2uUM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

Atmel 和 Arduino 在世界创客大会上合作推出了 [Wi-Fi shield 101](http://www.atmel.com/about/news/release.aspx?reference=tcm:26-63341) 。来自 Atmel 的[Gary]给了我们这个新防护罩及其组件的内幕。盾牌是一个相当简单的东西，只携带重要的设备:一个 Atmel [WINC1500](http://www.atmel.com/devices/atwinc1500.aspx) WiFi 模块和一个 [ATECC108 加密芯片。](http://www.atmel.com/devices/ATECC108.aspx)

WINC1500 本身就是一个漂亮的小 WiFi 模块。WINC 以高达 72 Mbps 的速度处理 IEEE 802.11 b/g/n。按照今天的标准，72Mbps 听起来可能不算多，但对于大多数嵌入式应用来说已经足够快了。WINC 处理无线连接的所有繁重工作。连接是通过 SPI、UART 或 I2C，尽管在 Arduino shield 上它将运行在 SPI 模式下。

ATECC108 是 Atmel“加密认证”系列的一员。它采用 8 引脚 SOIC 封装，与串行 I2C EEPROM 规格兼容。内部与串行 EEPROMs 的相似之处结束。‘108 在硬件上有一个 256 位的 [SHA](http://en.wikipedia.org/wiki/SHA-2) 引擎，以及一个[联邦信息处理标准(FIPS)](http://en.wikipedia.org/wiki/FIPS_140-2) 级别的随机数发生器。Atmel 认为这种芯片是安全嵌入式系统的核心。我们认为这非常好，只要我们在下一次 [DEFCON](http://hackaday.com/2014/08/09/defcon-22-hack-all-the-things/) 上不听到它。

Wi-Fi shield 101 和相关图书馆将于 2015 年 1 月推出。我们迫不及待地想看到所有的新项目(和闪烁 LED 的新方法)。