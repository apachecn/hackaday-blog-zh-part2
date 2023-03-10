# Raspberry Pi 蓝牙接收器，适用于您的汽车音响

> 原文：<https://hackaday.com/2014/06/23/raspberry-pi-bluetooth-receiver-for-your-car-stereo/>

![RasPi Car Audio](img/f333da3c378ba9a35b2808efc4ce60cf.png)

通过蓝牙连接在车内播放音乐非常方便。你通常只需打开手机的蓝牙模块，它就会自动与你的汽车配对。然后你所要做的就是加载一个音乐播放器应用程序，然后按下播放键。你不必担心每次上下车时都要把手机绑在车上。不幸的是，蓝牙不是许多汽车的标准选项，而且购买售后适配器可能会很贵。

[Parker reed][用树莓派为这个问题建立了自己的解决方案](http://www.reddit.com/r/raspberry_pi/comments/28ogmo/i_made_my_pi_an_incar_bluetooth_audio_receiver/ "RasPi car audio")。他首先在他的 Pi 上安装了 arch Linux。他还必须安装 pulseaudio 和 bluez，如果你使用软件包管理器，这是微不足道的。然后，他修改了一些 Linux 配置文件，以便在内核初始化之后自动将 Pi 的蓝牙适配器联机。

在引导序列结束时，Pi 被配置为以[Parker reed]用户的身份自动登录到虚拟控制台。然后，用户的 bashrc 文件被修改，以便在登录序列结束时以守护模式启动 pulseaudio。这允许 Pi 通过 Pi 的声卡实际播放音频。然后，使用标准音频电缆将 Pi 的立体声输出插孔插入车辆的辅助输入插孔。

Reddit 帖子包含了复制该设置所需的所有配置细节。[Parker reed]还包括一些命令，您将需要这些命令来设置 Raspberry Pi 与您的智能手机的初始配对。一定要看下面的视频演示。

[https://www.youtube.com/embed/6zprvj1SdVg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6zprvj1SdVg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/raspberry_pi/comments/28ogmo/i_made_my_pi_an_incar_bluetooth_audio_receiver/ "Reddit.com")