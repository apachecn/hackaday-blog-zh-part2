# 乐谱到 MIDI 转换器

> 原文：<https://hackaday.com/2014/12/22/sheet-music-to-midi-converter/>

学习阅读乐谱对新音乐家来说是一个挑战，所以康奈尔大学的一群学生决定让机器人来代替。对于他们的最终项目，他们建造了一个[机器人乐谱阅读器](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/dy264_ly288_yh644/dy264_ly288_yh644/project.html)(链接警告:该页面在加载时似乎会自动开始下载. mov 文件)。

作为输入，机器人拿起一卷钢琴。这是一张长纸条，上面印有音乐，可以很容易地通过阅读器输入。旋转伺服系统使纸带以恒定的速度传送，并使其通过阅读器。

读取器基于 Melexis [MLX75306](http://www.melexis.com/Optical-Sensors/Optical-Sensing/MLX75306-771.aspx) 线性光学阵列。该 IC 是一个 142 x 1 光电二极管阵列，设计用于汽车燃油质量检测。在这个项目中，它被重新设计成一个摄像头，在音乐经过时读取音乐。led 阵列照亮钢琴卷，提供更准确的读数。

这些部件连接到一个 Atmel [ATmega1284P](http://www.atmel.com/devices/ATMEGA1284P.aspx) 上，它完成所有需要的控制和处理。它创建钢琴卷帘窗的 MIDI 输出，可以连接到任何硬件或软件合成器。