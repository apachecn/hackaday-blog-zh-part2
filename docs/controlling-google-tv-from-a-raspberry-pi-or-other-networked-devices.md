# 从 Raspberry Pi(或其他联网设备)控制谷歌电视

> 原文：<https://hackaday.com/2012/11/01/controlling-google-tv-from-a-raspberry-pi-or-other-networked-devices/>

![](img/fb77be1b0c403be7209d45b4886b218f.png "rpi-controlling-a-googletv")

谷歌电视是一款联网电视。它的功能和你想象的一样:播放电视节目，从互联网上下载流媒体，并允许你在电视上打开网址。但一个很好的特点是，它也可以通过网络控制，而不仅仅是通过红外遥控器。谷歌发布的应用程序让智能手机变得简单。但是通信协议是开源的，所以【Leon Nicholls】用 Java 写了[一个谷歌电视遥控库。](https://github.com/entertailion/Anymote-for-Java)

广告之后的视频显示，他将一个树莓派与他的电视配对。上图是授权控制前您必须在远程硬件上输入的配对验证码。显然，如果使用谷歌的 Anymote 库，这是每次都需要进行的一步。[Leon]通过保存配对数据改进了这一点，这样只需第一次授权即可。

他认为这可以用于家庭自动化。我们不确定我们会用它做什么，但我们很乐意在评论中听到你的想法。