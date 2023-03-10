# 树莓 Pi 作为 XBMC 硬件达到临界质量

> 原文：<https://hackaday.com/2012/11/19/raspberry-pi-reaches-critical-mass-as-xbmc-hardware/>

多年来，我一直梦想有一种流媒体设备，可以贴在电视机的背面。由于 XBMC 一直是我最喜欢的机顶盒软件，我一直密切关注可以运行该软件包的硬件开发。现在，我认为是时候宣布树莓 Pi 已经达到了基本规格，被命名为统治它们的 XBMC 设备。

关于这个话题有各种各样的观点，但是请在休息之后听我说完，看看是什么让我得出这个结论。

## 媒体播放和高清

当我第一次在 Raspberry Pi 上试用 XBMC 时，我惊讶地得知该板没有 MPEG-2 硬件解码功能。这是一个巨大的交易断路器，因为我录制的一切空中(使用 ATSC 调谐器和 MythTV)使用的编解码器。这个问题已经解决了。花几块钱(我想它花了我 3.30 美元)你现在就可以[购买一个极其容易安装](http://www.raspberrypi.org/archives/1839)的许可证。我用 Paypal 支付，然后将发送给我的代码复制粘贴到 SD 卡的文本文件中。

现在，RPi 可以轻松播放 1080i mpeg 录像。我正在运行 OpenElec，甚至有人支持将 XBMC 作为 PVR 的前端(MythTV 插件还没有做好 beta 测试的准备，但很快就会了)。

## 控制选项

[![](img/5a3cfa07c9507aa111c38dd6b2b0bc1f.png "hdmi-cec-remote")](http://hackaday.com/?attachment_id=90331)

该板有多种控制选项，但我认为最好的是消费电子控制( [CEC](http://en.wikipedia.org/wiki/Consumer_Electronics_Control#CEC) )。这可以让你用电视通过 HDMI 线控制 XBMC。不是所有的电视都有这个，但是我的有。这里看到的遥控器有方向按钮、OK、菜单、返回、这四个彩色按钮、数字键盘和底部的 DVR 控件(播放、暂停、停止等)。).这在 OpenElec 的最新版本中自动启用，以实现一些零配置的优点。

就像所有 XBMC 的现代建筑一样，你可以通过家庭网络来控制它们。你可以在 Android 和 iPhone 上使用 XBMC 远程应用程序，甚至可以编写自己的程序。

[![](img/c07a400f5e427995d58704972353ade3.png "rpi-ir-remote-receiver")](http://hackaday.com/?attachment_id=90332) 这是一个 Linux 发行版的事实意味着它甚至可以使用 lirc。这是一个长期以来用于为家庭影院电脑添加红外遥控器的包。我记得用 V-USB 堆栈和 ATtiny2313 构建了自己的 USB IR 接收器。但是这种类型的工作并不要求将 IR 接收器连接到 RPi。得益于 GPIO 头，您可以非常轻松地启动和运行。我手头有一个 TSOP4838。这在 5V 电压下运行，该电压可由割台提供。但是 RPi 上的 I/O 引脚不能承受 5V 电压，所以我在信号引脚上加了一个分压器。我发现这个[帖子对让接收器和 Lirc 工作](http://aron.ws/projects/lirc_rpi/)有极大的帮助。

## 费用

我想考虑的最后一个方面是设备的成本。有了 Raspberry Pi 板、电源和解码器许可证，价格都在 100 美元以下，你怎么会出错呢？我敢打赌，你可以买一个漂亮的小箱子，但仍然不会超过一个本杰明门槛。

## 结论

[![](img/879b84bcaac1c310b6b6d974c6f76e60.png "rpi-zip-tied-to-entertainment-center")](http://hackaday.com/2012/11/19/raspberry-pi-reaches-critical-mass-as-xbmc-hardware/rpi-zip-tied-to-entertainment-center/)

我用于测试的软件都处于开发阶段，但一切似乎都很好。如我所说，高清视频播放流畅。XBMC 的附加组件在菜单中运行得有点慢，但是回放很完美。

正如您在这里看到的，我将进行一些长期测试。我没有用 Velcro 把主板固定在电视机的背面，而是用拉链把它绑在了我的娱乐中心的下面。我还没有算出这个东西在不使用时会消耗多少电力，但确实没有休眠的选项(问题在于从断电状态中醒来)。我不确定这是否会在未来得到解决，但目前我只是在用完设备后拔掉它。在我看来，这是一个小问题，可以通过智能电源板来解决，它可以在电视关闭时进行切换。我将拭目以待，看看在不久的将来是否会出现更有说服力的解决方案。

我觉得有必要提一下，我很乐意在这个设备上播放网飞的视频。但这是网飞的不足，而不是 XBMC 或树莓派的不足。它应该可以通过非官方的插件播放 Hulu Plus 和 Amazon Prime。