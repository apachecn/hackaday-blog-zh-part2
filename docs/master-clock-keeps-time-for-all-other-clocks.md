# 主时钟为所有其他时钟计时

> 原文：<https://hackaday.com/2014/09/04/master-clock-keeps-time-for-all-other-clocks/>

[Brett]刚刚完成这款[极其精确的时计](http://home.btconnect.com/brettoliver1/Master_Clock_MK2/Master_Clock_MK2.htm)的建造和长期测试。它通过定期与德国 Mainflingen 的原子钟同步来保持时间。

该项目的核心是 ATMega328，它使用新的 [DCF77 库](http://blog.blinkenlight.net/experiments/dcf77/dcf77-library/)来解码原子钟广播的信号。Udo Klein 编写的库显著提高了读取信号的器件的噪声容限，但它们不适用于任何使用谐振器而非晶体的项目。

在原子钟完全失去信号的情况下，驱动时钟的微处理器还有一个备份晶体，可以保持时钟每天运行 1 秒钟以内的精度。这个时钟也可以驱动从时钟，根据[Brett]需要它们做什么，使用不同定时的脉冲。显示屏也很不错:六个七段显示屏显示时间，一个 LCD 面板读出时钟数据。它甚至有整点和一刻钟的报时功能，而且还有很多其他功能！

关于计时最烦人的事情之一是[夏令时校正](http://hackaday.com/2012/07/16/automatic-daylight-savings-time-compensation-for-your-clock-projects/)，这个时钟用一个手动开关来处理它。这可以真正照顾到你所有的计时需求！