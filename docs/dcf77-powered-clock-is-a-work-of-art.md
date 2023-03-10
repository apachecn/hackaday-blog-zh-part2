# DCF77 供电时钟是一件艺术品

> 原文：<https://hackaday.com/2013/12/06/dcf77-powered-clock-is-a-work-of-art/>

[![](img/0e3527faa8a737733751a9f7f327c2b7.png)](http://hackaday.com/wp-content/uploads/2013/12/lcd_master_clock.jpg)

【Brett】刚刚完成他的 [DCF77 主支架时钟](http://home.btconnect.com/brettoliver1/LCD_Master_Clock.htm)，打算作为他做的的[老逻辑控制时钟的备份。对于我们不知道的读者来说，](http://home.btconnect.com/brettoliver1/masterclock.htm) [DCF77](http://en.wikipedia.org/wiki/DCF77) 是一个德国长波时间信号，其发射机位于法兰克福(德国)附近。每分钟，当前日期和时间都在 77.5kHz 载波信号上发送。

你可以在上面看到的结果，是使用一个 Ikea lantern、一个骨架时钟、一个 ATmega328(兼容 Arduino)、一个录音回放 IC (ISD1730)、一个廉价的 20×4 LCD 显示器、一个 DCF77 接收器模块和许多 led 制成的。我们很确定[布雷特]一定花了很长时间才得到这么好看的钟。万一时钟失去电源，3 节 AA 电池提供备用电池。在固件方面，使平台兼容 Arduino 允许[Brett]使用它的库，所以编码很快就完成了。休息后嵌入的是最终结果的视频。

[https://www.youtube.com/embed/Pye6zYBQjiY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Pye6zYBQjiY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)