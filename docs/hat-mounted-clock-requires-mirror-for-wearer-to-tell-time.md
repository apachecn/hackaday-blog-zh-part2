# 戴在帽子上的钟需要镜子来告诉佩戴者时间

> 原文：<https://hackaday.com/2015/02/14/hat-mounted-clock-requires-mirror-for-wearer-to-tell-time/>

[gfish]计划参加燃烧的人，并想做一些独特的(和有用的)穿。他决定买一个帽子和时钟的混合体。不过，只是在帽子上盖一个钟太容易了。[gfish]希望他的帽子可以通过手动开关或物理位置来改变时区。

和大多数钟表一样，帽子的正面有 2 根指针。每一个都连接到帽子后面的两个同心轴中的一个上。每只手都由遥控车辆伺服系统单独控制。熟悉遥控伺服系统的人都知道，伺服系统的最大旋转角度约为 180 度，当然不足以完成时钟所需的完整旋转。为了解决这个问题，有一个 3:1 齿轮组，允许 120 度的伺服旋转，以移动时钟指针整整 360 度。使用这种方法，每根指针都不能移动超过 12 点，而是必须快速逆时针移动到需要的位置，以便再次开始围绕钟面的旅程。

帽子里安装了一个 Arduino 来控制时钟，一个 GPS 屏蔽来确定位置，一个 RTC 来保持准确的时间。安装在帽子侧面的是一个控制面板，它包含一个总的开/关开关以及一个用于选择特定时区或启用 GPS 模式的旋转开关。整个装置由 9 伏电池供电。

如果你喜欢不必要的复杂礼帽，看看这个显示 one 的 [WiFi 启用信息。](http://hackaday.com/2014/08/01/defcon-shenanigans-hack-the-hackaday-hat/)

[https://www.youtube.com/embed/7Y-8bhTzjd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7Y-8bhTzjd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)