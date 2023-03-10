# 在这个声控 3D 扫描设备上旋转一下

> 原文：<https://hackaday.com/2015/03/22/take-a-spin-on-this-voice-controlled-3d-scanning-rig/>

[Aldric Negrier]想让三维扫描人变得简单而流畅。为此，他创造了这个声控 3D 扫描设备。

[Aldric]使用了各种各样的黑客技术来完成这个项目，他的详尽说明很好地说明了这一点。从数控铣削到 Arduino 编程到 3D 打印，一切都融入了这个钻机的制作中。胶合板被用来建造基地和大齿轮。一个 12 英寸的转盘轴承连接到这个齿轮上，以允许平稳旋转。为了实现钻机的自动化，一个 12V 的 DC 齿轮电机被连接到一个更小的 3D 打印齿轮上，并放置在底座上。当马达启动时，小齿轮的齿带动大齿轮旋转。他使用了一个朋友制作的定制双 H 桥电机驱动器，该驱动器连接到一个 Arduino Nano。Nano 还连接到蓝牙模块和超声波测距仪。当在 3 秒钟内检测到钻机上 1-35 厘米范围内的物体时，电机开始旋转，当不再检测到物体时停止。典型的扫描大约需要 60 秒。

这本身就是一个伟大的工程，但是[奥德里奇]并没有就此止步。他希望能够在被扫描的同时踩在钻机上并发出命令。如果你想对自己进行扫描，这是有意义的——登上平台，找到想要的位置，然后开始扫描。他使用 Windows 语音识别 SDK 开发了一个应用程序，通过蓝牙向 3D 扫描软件[sk anet](http://skanect.occipital.com)发出命令。命令就像说“启动 Skanect”一样简单你也可以告诉电机打开或关闭，并改变其速度或方向，而不破坏形式。【奥德里奇】使用了一台[华硕 Xtion](http://www.asus.com/Multimedia/Xtion/) 作为 3D 扫描仪，但一台 [Kinect](hackaday.com/2014/03/09/kinect-wiper-motor-lego-3d-scanner/) 也能工作。之后，他使用 [MeshMixer](http://www.meshmixer.com/) 平滑扫描，这是一个在[之前的](hackaday.com/2014/06/22/converting-cts-and-mris-into-printable-objects/) [黑客](hackaday.com/2014/10/13/3d-printing-models-from-computer-games/)中出现的程序。

休息后，请查看钻机的视频。由于其中一个视频中的背景音乐，语音命令很难听到，但如果你仔细听，你可以听到它们。你还可以在这里或者在这个 [YouTube 频道](https://www.youtube.com/channel/UCDxekuZzOMzEuBkfMC3-j_Q)上看到更多【奥德里奇】的项目[。](http://www.reprapalgarve.com)

[https://www.youtube.com/embed/-wOqgN9tUXU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-wOqgN9tUXU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/BLVS36rh6c4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BLVS36rh6c4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢你的提示，梅洛佛！]