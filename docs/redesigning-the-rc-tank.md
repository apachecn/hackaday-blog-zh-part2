# 重新设计遥控坦克

> 原文：<https://hackaday.com/2012/07/21/redesigning-the-rc-tank/>

[https://www.youtube.com/embed/--YZHMqHzPw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/--YZHMqHzPw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[文森特]开始建造这种坦克 ( [翻译](http://translate.google.com/translate?sl=fr&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fwww.bricobidules.com%2Findex.php%3Fpost%2F2012%2F02%2F28%2FUn-robot-qui-%25C3%25A9vite-les-obstacles))有一个固定的爱好模型:[恒隆虎 1](http://www.amazon.co.uk/Heng-Long-German-Tiger-Control/dp/B0037Q9KPU) 。然而，在考虑了这个项目的一些目标后，他决定几乎掏空这个坦克，并基于 Arduino 和一个标准的电机护罩对它进行重新设计。这种设置的可能性几乎是无限的。在目前的形式下，ArduTiger 通过三个安装在伺服系统上的红外测距仪来探测前方的障碍物。坦克的轨迹可以根据伺服位置的反馈自动调整。两个额外的短程测距仪检测是否有地面可供坦克翻滚，使其免受悬崖和黑洞的威胁。[Vincent]计划通过添加一个用于实时视频和高级控制的[树莓 Pi](http://www.raspberrypi.org/) 来更新这个怪兽…甚至可能添加一个盖革计数器！