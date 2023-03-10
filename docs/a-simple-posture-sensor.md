# 一个简单的姿态传感器

> 原文：<https://hackaday.com/2014/02/18/a-simple-posture-sensor/>

![ChairPosture](img/865967aaa9d62ed9609999157cdb49ac.png)

如果你一天的大部分时间都在电脑前，姿势会成为一个严重的问题，会对你的健康产生负面影响。[僚机]看到了这个问题，并创造了一个黑客来帮助解决它。他的[简易姿势传感器](http://coretechrobotics.blogspot.de/2014/02/a-very-simple-posture-sensor.html)会监测你的头部相对于椅子的位置，并提醒你坐直。

姿态传感器围绕 [HC-SR04](http://www.instructables.com/id/Easy-ultrasonic-4-pin-sensor-monitoring-hc-sr04/) 超声波距离传感器、 [Attiny85](http://www.atmel.com/devices/attiny85.aspx) 和压电扬声器构建。我们已经看到这种距离传感器[在过去](http://hackaday.com/2013/04/30/sump-pump-alarm-sends-text-message-as-water-rises/)用于[少数项目](http://hackaday.com/2013/12/03/a-speaking-ultrasonic-distance-sensor/)。[僚机]决定将传感器安装在椅背上，而不是走可穿戴路线，因为可穿戴路线有其自身的缺点。最棒的是，传感器不是直接安装在椅子上，而是安装在一块织物上，这样在需要时就可以轻松移动。

鉴于传感器的低成本和小尺寸，该项目可以通过在不同位置添加多个传感器来轻松扩展。这将允许确定背部和可能的颈部的角度，给出不良姿势的更准确的指示。很少有解决不良姿势的方法。你有帮助解决不良姿势的项目吗？你使用过视频处理或可穿戴设备来监控你的姿势吗？请在评论中告诉我们，不要忘记将关于它们的帖子链接发送到我们的提示热线。