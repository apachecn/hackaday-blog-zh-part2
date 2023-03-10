# Raspberry Pi 作为 Spotify 服务器，带有 MPD 控件

> 原文：<https://hackaday.com/2013/03/14/raspberry-pi-as-a-spotify-server-with-mpd-control/>

Raspberry Pi 作为流媒体音乐播放器非常受欢迎。当然，板上唯一的音频输出选项是模拟立体声插孔，但如果你愿意，你可以使用 USB 音频设备来改善这一点。[Wouter van Wijk]希望将他的 RPi 用作 Spotify 服务器。为此配置好一切有点棘手，所以他决定通过为树莓 Pi 发布[一个可以使用的 Spotify 服务器图像](http://www.woutervanwijk.nl/pimusicbox/)来回报。

该项目被称为 Pi 音乐盒。像一些 RPi Pandora 设置一样，我们已经看到他也包括了将硬件作为 AirPlay 设备的能力。为了连接 Spotify 服务，他使用了[的 Mopidy 包](http://www.mopidy.com/)。它还可以播放本地存储器(包括家庭网络)中的曲目。它甚至能够在同一个队列中混合两种来源。可能最好的部分是，它可以用任何音乐播放器守护程序(MPD)客户端控制，就像上面看到的智能手机截图一样。

如果你感兴趣，可以看看[为项目](https://github.com/woutervanwijk/Pi-MusicBox)准备的 GitHub 回购。