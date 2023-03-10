# 更新:LED 条形显示屏上播放的实时视频

> 原文：<https://hackaday.com/2013/05/26/update-live-video-played-on-led-strip-display/>

![update-live-video-on-led-strip-display](img/9d957ac73029000c461d70ca8a535305.png)

[Paul]带着这个 LED 显示屏去了 Maker Faire。为了给它一些交互性，他想出了一个让它播放现场视频的方法。它还可以使用一些由压电扬声器元件和橡胶地板垫制成的踏脚执行器来激活。

这使他最初的项目朝着新的方向发展。早在二月份，他就[展示了 RGB LED 条形显示屏](http://hackaday.com/2013/02/25/building-huge-displays-with-led-strips/)。他让它播放视频，但这都依赖于使用以前处理过的文件。这次升级使用了[一种比格犬骨黑](http://beagleboard.org/Products/BeagleBone%20Black)(基于 ARM 的开发板的最新版本)。[Paul]曾尝试使用 Raspberry Pi 板，但网络摄像头(安装在 LED 显示屏上方)出现丢帧问题。有了新的板，他能够使用 Video4Linux API 每秒捕捉 30 帧，并将其推送到显示器上。

到目前为止，1920 个发光二极管中有 5 个死在他身上。这展示了使用这样的条带的一些好处。一个坏像素不会影响它的邻居。更换非常简单，只需剪断坏部件两侧的带子，然后在适当的位置焊接一个新部件。