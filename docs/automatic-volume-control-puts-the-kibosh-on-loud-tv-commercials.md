# 自动音量控制杜绝了喧闹的电视广告

> 原文：<https://hackaday.com/2013/02/11/automatic-volume-control-puts-the-kibosh-on-loud-tv-commercials/>

![automatic-tv-volume-control](img/0b10bfec4d97bf7d4cb81aa7f52c4ecb.png)

如果你很难不去理会那些喧闹的商业广告，为什么不让你的电子项目为你做呢？这是一个基于 Arduino 的设置，当电视音量超过某个阈值时[会调整电视音量。它使用麦克风，而不是直接的音频信号，因此您可以根据房间内实际听到的声音进行设置。](http://www.instructables.com/id/TV-Volume-Loudness-Guard-using-Arduino)

控制方案使用 IR LED 和 IR 接收器，如上面的试验电路板电路所示。接收器可让您将遥控器上的音量调高和调低按钮教给系统。我们在设计中看到的一个缺点是音量级别是硬编码的，需要您刷新新代码来进行调整(也许有事业心的读者可以添加一个电位计来轻松调整？).

我们不禁想起了[读取隐藏字幕信息来屏蔽你添加到黑名单](http://hackaday.com/2011/08/16/automatically-weed-the-celebrity-gossip-out-of-your-tv-time/)中的话题的设置。