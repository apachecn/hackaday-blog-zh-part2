# 用手的挥动来控制音乐

> 原文：<https://hackaday.com/2014/08/06/controlling-music-with-the-wave-of-a-hand/>

![2301141406514425783](img/f668a2ae2e151be85f3448ae834d389c.png)

[托马斯]创造了一个神奇的音乐播放器,让听众能够改变歌曲和音量，而不必接触除了空气以外的任何东西。这款设备名为 LighTouch，通过解释来自超声波传感器的输入，将控制权放在用户手中，并根据挥手手势播放曲目。

这是他大约一年前完成的原型的第二次迭代，功能是流式收音机/闹钟。该传感器被连接到一个带有褪色 LED 的树莓皮上。一切都是高度可定制的，包括用于回放功能的距离。[Thomas]提出的标准是，当在距离传感器 0-10 厘米处检测到物体时，会触发暂停方法。下一个级别的音量控制可以使 LED 灯变亮或变暗，只是为了增加一些特色。

![9120061407006675261](img/ea43457979cead017907076f94fe2967.png)

此外，[Thomas]还集成了一个 LCD 屏幕来显示当前播放的曲目。Pi Alamode GPIO 屏蔽充当 Raspberry Pi 和超声波传感器/LCD 之间的接口。定制的焊接板也用于确保外壳内的正确放置。播放列表也可以设置。[Thomas]建议使用 [MPDroid](https://play.google.com/store/apps/details?id=com.namelessdev.mpdroid&hl=en) 来实现这个功能。

这是[Thomas]演示 LighTouch 的视频:

[https://www.youtube.com/embed/ZCrYmi5ZA3M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZCrYmi5ZA3M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)