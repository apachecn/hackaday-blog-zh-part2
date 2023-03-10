# 使用 Arduino 拨打手机

> 原文：<https://hackaday.com/2012/09/03/make-cell-phone-calls-with-your-arduino/>

Arduino 的蜂窝屏蔽已经存在很长时间了，但[这是我们看到的第一个把你的 Arduino 变成一部真正的手机的手机。](http://www.open-electronics.org/gsm-gps-shield-for-arduino/)

该防护罩基于 [SIM900 GSM/GPRS](http://store.open-electronics.org/Modules/GSM%20modules/SIM900%20-%20Quad-band%20GSM_GPRS%20module) 无线电模块，并与添加了 GPS 接收器的 [SIM908 GSM/GPRS](http://store.open-electronics.org/Modules/SIM908_GSM_GPRS_GPS) 模块兼容。该保护罩上还有一对 1/8”音频插孔，非常适合连接麦克风和耳机。是的，你现在可以用 Arduino 打手机了。

这个构建的真正明星是新的 [GSM 盾库](http://code.google.com/p/gsm-shield-arduino/)。这个代码库包括 Arduino 作为手机使用所必需的方法(接听、挂断、拨号)，还包括许多对 TCP/IP 通信的改进。

尽管让 Arduino 通过 GSM 或 GPRS 网络进行通信的成本相当高，但我们认为这将是完全开源、开放硬件手机的完美起点。一部功能与同样是 MiFy 的老诺基亚砖相同的手机将是一件令人惊叹的硬件，肯定会成为一个有利可图的 Kickstarter。