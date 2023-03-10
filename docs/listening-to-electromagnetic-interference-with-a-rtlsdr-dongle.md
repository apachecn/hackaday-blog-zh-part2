# 用 RTLSDR 加密狗监听电磁干扰

> 原文：<https://hackaday.com/2014/03/18/listening-to-electromagnetic-interference-with-a-rtlsdr-dongle/>

[![](img/33c1b043657e61c181b0b90a35ddbc98.png)](http://hackaday.com/wp-content/uploads/2014/03/2014-03-09-fast-pwm-emi-the-lab.jpg)

天生好奇，[Marios]决定看看连接到简单试验板电线的 Arduino 可能会产生何种无线电频率发射，更重要的是，尝试使用 RTLSDR 加密狗拾取它们。电磁干扰是由于[电磁感应](http://en.wikipedia.org/wiki/Electromagnetic_induction)或[电磁辐射](http://en.wikipedia.org/wiki/Electromagnetic_radiation)而影响电路的干扰。在进入市场之前，所有的电气设备都经过了彻底的检查，以防止有害的电磁辐射，因此当出现此类问题时，它们通常不是显而易见的嫌疑对象。

在快速 PWM 模式下使用 Arduino embedded [PWM](http://en.wikipedia.org/wiki/Pulse-width_modulation) 控制器，并通过操纵占空比，他实际上成功创建了一种原始形式的幅度调制，并能够在高达 1.75GHz 的几个频率下传输非常简单的音频信号。休息后嵌入的是系统工作时的视频。

顺便提一句，你知道吗，在 1859 年[太阳风暴](http://en.wikipedia.org/wiki/Solar_storm_of_1859)期间，电磁干扰非常强烈，电报员受到了几次电击。管道维护系统也必须意识到这种事件，这可能导致传感器提供不准确的结果。

[https://www.youtube.com/embed/fvQ7NFbLy3w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fvQ7NFbLy3w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [危险原型](http://dangerousprototypes.com/2014/03/14/fast-pwm-and-electromagnetic-interference/)