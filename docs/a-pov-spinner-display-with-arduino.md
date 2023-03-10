# 使用 Arduino 的 POV 微调器显示

> 原文：<https://hackaday.com/2013/11/18/a-pov-spinner-display-with-arduino/>

![pov-display](img/4a2a3a75bb53f6974df2f9f1c0bb34e2.png)

[Martin2250]一直在研究一种[旋转圆盘风格的视点显示](http://imgur.com/a/LLmQM/#0)。他[在 reddit](http://www.reddit.com/r/arduino/comments/1qtrki/spinning_disk_pov_display_finished_details_in/) 上发布了他的进展。这个技巧是一个很好的例子，说明了如何使用您所拥有的资源。[Martin2250]使用红外 LED 和光电二极管来确定光盘的转速。他尝试使用 Arduino micros()函数来延迟光电二极管脉冲和打开 led 之间的时间。正如[Martin2250]发现的那样，micros()对于这个目的来说不够准确。他后来转而使用 AVR 的本地定时器，并且取得了更好的效果。

这个版本中光盘实际上是一张 CD。打磨掉标签，然后掩盖他的数字。他用黑色记号笔在光盘上“涂色”。剥去胶带，露出了他程式化的数字。纸板、热熔胶和可见发光二极管被用来为数字创建四个灯箱。光盘可以同时显示任意四个数字，非常适合 POV 时钟。我们喜欢在这个作品中使用现成的材料——硬木和轻木，大量使用热熔胶，当然还有纸板。我们眼中唯一缺少的就是一些胶带！

[https://www.youtube.com/embed/_0pcCUg3ngc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_0pcCUg3ngc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)