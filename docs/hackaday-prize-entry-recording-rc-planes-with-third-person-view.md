# Hackaday 奖参赛作品:用第三人称视角记录遥控飞机

> 原文：<https://hackaday.com/2015/06/18/hackaday-prize-entry-recording-rc-planes-with-third-person-view/>

随着小型廉价视频发射器的最新进展，第一人称视角遥控飞机如此受欢迎也就不足为奇了。这是进入驾驶舱最简单的方法，而不必花费数千美元和 50 个小时左右的时间去考飞行员执照。尽管 FPV 飞行面临着各种技术挑战，但记录遥控飞机仍有一个不足之处:第三人称视角，或者更普遍的说法是，“把摄像机交给你的朋友”

[沃克·埃里克]想做些什么。他一直想要他驾驶飞机的漂亮视频，但他不能一边拍摄一边飞行。他*可以*制造一个机器人，[这是他参加黑客奖](https://hackaday.io/project/5985-autonomous-video-recording)的参赛作品。

[Walker]的项目使用了一个基站和一个安装在万向架上的摄像机。这种设置的电子设备出奇地简单——只需一个 GPS 信标将遥测数据向下传输到基站。通过将这些数据与地面站上的 GPS 接收器进行比较，可以计算出飞机的方向。

这种设置存在一些问题。用 GPS 测量高度不是很精确，所以[Walker]在 GPS 信标上使用一个压力传感器作为高度计。当前的设置工作得很好，并且比在转向 GPS 之前测试的 OpenCV 设置有了很大的改进。

[Walker]已经有一些令人难以置信的视频，他用这个系统在他的本地场地周围驾驶一些飞机和飞行器。你可以看看下面这些。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/UB5F9ri8P08?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UB5F9ri8P08?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/e3tu5ZIehTw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/e3tu5ZIehTw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)