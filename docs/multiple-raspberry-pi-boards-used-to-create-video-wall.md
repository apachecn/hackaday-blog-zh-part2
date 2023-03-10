# 用于创建视频墙的多个 Raspberry Pi 板

> 原文：<https://hackaday.com/2013/07/22/multiple-raspberry-pi-boards-used-to-create-video-wall/>

五个 Rasberry Pi 用于驱动[这个四显示器视频墙](https://www.dropbox.com/s/0nu5p5fbu0vu35m/VIDEO0010.mp4)。这张截图显示了系统正在播放一些 BBC 纪录片。同步、对齐和视频质量似乎都很准确，这使得你的眼睛很容易将图像组合成一张图片。

每个屏幕都有自己的 Raspberry Pi，可以生成 HDMI 视频显示在屏幕上。这些信号由一个充当控制器的中央 RPi 板提供。视频通过 Linux GStreamer 包提供的实时流协议( [RTSP](http://en.wikipedia.org/wiki/Real_Time_Streaming_Protocol) )在电路板之间推送。不同视频板之间的同步使用网络时间来处理。[萨梅尔]提到这个系统是可扩展的—每个额外的屏幕只需要多一个 RPi 来驱动它。

该团队还用直播视频做了一些实验。他们添加了第六个带摄像头模块的 RPi 板，以便[显示实时反馈](https://www.dropbox.com/s/2fn8arb046jd0gh/VIDEO0012.mp4)。