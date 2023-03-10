# Hack-a-Day 徽标激光灯光秀

> 原文：<https://hackaday.com/2013/11/24/hack-a-day-logo-laser-light-show/>

[![hackaday-laser-2](img/11e5b6e8de4912f4544e6eea00c72700.png)](http://hackaday.com/wp-content/uploads/2013/11/hackaday-laser-2.jpg)

“一天黑一个 logo”的挑战不断取得成果。这条建议来自阿根廷的[Enrico Lamperti],他发布了自己使用自制的扫描激光投影仪成功创建了一个 [Hack-a-Day logo。](http://blog.elamperti.com/2013/11/drawing-with-a-laser/)

该建筑由几个小型伺服系统、一个被黑掉的笔式激光器和一个 Arduino 组成，Arduino 带有一些存储的坐标来绘制图像。像往常一样，第一个挑战是给你的外围设备供电，比如伺服系统。[Enrico]使用 6 节镍氢电池和一个 LM2956 简单开关电源转换器解决了这个问题。伺服系统和 Arduino 直接从电池组获得电力，Arduino 控制伺服系统的 PWM 信号，因为它们跟踪存储的坐标数据。激光器连接到伺服组件，由 Arduino 引脚通过 NPN 晶体管接合和供电。他还加入了一个电位计来调整伺服校准点。

他第一次导入从 Python 脚本生成的坐标数据并不成功。但后来他用 SVG 文件处理了一条点击路径，Arduino 可以用这条路径作为地图数据来绘制 Hack-a-Day 徽标。在暗室中拍摄完整的图画需要很长的曝光时间，但效果令人印象深刻。

这是一个很好的项目，其中[Enrico]分享了他关于使用 Servo.write 微秒()而不是 servo . write()来提高性能的经验，以及其他一些调整。他还在 GitHub 上分享了 BOM、Fritzing 图、Processing Creator 和 Simulator 工具以及串行命令[。他总结了一些他认为可以改进他的设备的选项，并请求其他人提供任何帮助以提高性能。如果你愿意，你可以更上一层楼，用 ATMega16 AVR 微控制器和一些聪明的旋转倾斜镜创造一个](http://github.com/elamperti/laserdriver)[激光视频投影仪](http://hackaday.com/2007/01/04/avr-laser-projector/)。