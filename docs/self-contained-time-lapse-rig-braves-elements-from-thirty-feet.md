# 独立的延时摄影装置可以从 30 英尺的高空拍摄

> 原文：<https://hackaday.com/2013/07/30/self-contained-time-lapse-rig-braves-elements-from-thirty-feet/>

这幅图中的透视有点难以把握，但所有这些硬件都安装在离地面 30 英尺的地方。这个延时摄影盒[利用阳光和树莓皮](http://imgur.com/a/Qwe82/layout/blog)来记录这一切。该钻机是[Patty Chuck]建造的三个之一，用于记录 18 个月来 70 英亩建筑工地的进展。上面链接的图库很好地展示了这个项目，但是在他的 Reddit 帖子中可以找到更深入的文字描述[。](http://www.reddit.com/r/DIY/comments/1ijayj/time_lapse_camera_system_selfsustaining_longterm/)

图像中没有显示的是为盒子供电的太阳能电池板。安装时，现场没有公用设施。为了防止断电，有一个硬件 RTC 一直在运行。在工作日，Raspberry Pi 使用 GPIO 引脚每五分钟打开一次尼康 D7100 相机。它会在再次关机前先拍照。它还监控温度传感器，并在必要时启动循环风扇。

他计划在 18 个月后项目完成后发布视频。如果你看到他们并记得这篇文章，[给我们发送链接](http://hackaday.com/contact-hack-a-day/)，我们将发布更新。