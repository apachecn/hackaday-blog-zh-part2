# 电脑播放 Flappy Bird。天网即将启动。人类挥舞着手臂。

> 原文：<https://hackaday.com/2014/02/28/computers-playing-flappy-bird-skynet-imminent-humans-flapping-arms/>

![flappy-double](img/38c31342ee389045e5a3c16dbad27d5e.png)

在病毒式的流行、开发者的愤怒退出以及疯狂的易贝拍卖之后，这个世界基本上就要结束 Flappy Bird 了。在 Hackaday，我们不能不展示两个以上的黑客。第一个是我们一直在等待的:一个会为我们玩该死的游戏的机器人。你的眼睛没有在那个标题图像中欺骗你。Flappy Bird 机器人已经达到 147 分，并且势头强劲。两名来自中国的黑客[史雪坤]和[刘洋]已为此次黑客攻击承担全部责任。他们在 Ubuntu 上使用带有摄像头的 OpenCV 来确定鸟和管道的位置。一旦知道了位置，计算机就会计算下一步行动。当需要拍打翅膀时，一个信号会被发送到 Arduino Mega 2560 上。这种黑客的天才之处在于执行器。大多数伺服系统或马达对于这种应用来说太慢了。(石)和(刘)使用 Arduino 和电机驱动器激活硬盘音圈。音圈速度很快，足以在准确的时间触摸屏幕，但没有强大到粉碎他们的平板电脑。

如果你想让拍打翅膀更像是一件身体上的事情，[Jérémie]用 Kinect 创造了 [Flappy Bird。](http://www.badbauds.io/2014/02/playing-flappy-bird-with-kinect-part-2/)他写了一个快速处理草图，使用微软 Kinect 寻找挥动手臂的人。如果检测到拍打，就会向 Android 平板电脑发送命令。[Jérémie]最初想使用 Android Debug Bridge (ADB)来发送触摸命令，但发现它对于这种硬核游戏来说太慢了。解决方法是使用串行连接的 Arduino 作为鼠标。加工草图通过串行向 Arduino 发送一个“#”。Arduino 然后向运行 [hidclient 的电脑发送鼠标点击。](http://anselm.hoffmeister.be/computer/hidclient/index.html.en) Hidclient 最终将蓝牙鼠标点击发送到平板电脑。诚然，这有点像 Rube Goldberg 的方法，但它确实[给 Flappy Bird hack](http://hackaday.com/2014/02/20/real-life-flappy-bird-in-a-box/) 添加了一个 Arduino，我们认为这是一个完美的配对。

[https://www.youtube.com/embed/kHkMaWZFePI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kHkMaWZFePI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/KqX6KxO7wJQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KqX6KxO7wJQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
【感谢帕克！]