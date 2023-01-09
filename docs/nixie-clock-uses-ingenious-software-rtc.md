# 谢妮时钟使用巧妙的软件 RTC

> 原文：<https://hackaday.com/2015/05/31/nixie-clock-uses-ingenious-software-rtc/>

数码管时钟有一点吸引着黑客们去构建他们自己的迭代，即使它已经被做过无数次了。它们不断耗尽的电源，以及控制它们的高压驱动器，让这一切变得更加有趣。[Pete Mills]是几个有趣项目的老手，其中许多我们已经在这里介绍过，他也不例外，并决定建立自己版本的[数码管时钟，但有几个漂亮的功能](http://petemills.blogspot.in/2015/05/nixie-tube-clock.html)。

简而言之，他的时钟使用谢妮电子管进行显示，具有 USB 串行通信、温度测量、交流频率测量、基于 RTC 的[软件保持时间和日期、用于 175V DC 数码管电源的软件驱动升压转换器和用于时钟配置的 windows 应用程序。](http://petemills.blogspot.in/2011/05/real-time-clock-part-1.html)

基于软件的计时非常有趣。它本质上是一种校准晶体以更好地匹配实时的方法，以及一些跟踪时间和日期的代码。这显然导致组件的减少以及随之而来的副产品；提高可靠性、降低成本、节省房地产。无论使用何种显示器，RTC 代码都可以轻松移植到其他时钟项目。除了跟踪时间和日期，它还可以考虑闰年，并报告星期几。连接到为时钟供电的低压变压器电源的过零检测器也可以用作保持时间的替代方法。

当通过 UART 连接到串行控制台时，时钟可以根据收到的查询报告许多变量。驱动谢妮电子管所需的高压 DC 由微控制器控制的简单升压转换器产生。[Pete]在烧断几个保险丝后得出的一个重要结论是，断开连接到 PWM 定时器的微控制器端口，并通过软件将其明确设置为低输出。他还遇到了一些其他问题，比如电路板布局、电源、不正确的上拉电阻，这些都是有趣的读物。时钟外壳仍在开发中，但[Pete]希望能尽快完成。

他还编写了一个 Windows 应用程序——谢妮时钟通讯器——来帮助设置和校准时间。最后，他详细描述了基于 RTC 的时钟软件校准过程。根据他的计算，在 8 个月的时间里，时钟将会漂移大约 48 秒。因为他将比这更快地适应夏令时，所以他的时钟在任何给定时间都应该与正确时间相差不超过一分钟。对于不使用专用 RTC 芯片的时钟来说，这已经不错了。[Pete]如果有人感兴趣的话，还有些原型板可以赠送。如果你宁愿自己从头开始建造它，[皮特]已经发布了[软件代码](https://github.com/pilotingpete)、[原理图和 PCB](https://docs.google.com/file/d/0B1CPUkh94AtmMmM5Y1NmeGttLWs/edit?usp=drive_web) ，以及一份 [BoM](https://docs.google.com/spreadsheets/d/1ZhO8OGlxGMYI7I5BOQ9BeYuwDf4MAAcQkCAm8IlP1JA/edit?usp=sharing) 。