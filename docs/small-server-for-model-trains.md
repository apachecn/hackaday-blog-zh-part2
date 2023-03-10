# 模型火车的小型服务器

> 原文：<https://hackaday.com/2012/10/26/small-server-for-model-trains/>

![](img/286c0f5246326b9a57c7ef3251d3e2e8.png "roc")

出于我们无法理解的原因，火车模型在德国非常流行。[Gerhard]是那些模型火车爱好者之一，他们已经远远超越了用变压器控制火车速度的布局；他向[提交了一个他建造的非常小的 Rocrail 服务器](http://lnxpps.de/can2udpe/smallest-rocrail-server-ever/)来控制机车在他的版图上移动。

[Gerhard]使用的是[Rocrail](http://wiki.rocrail.net/doku.php)——一种控制系统，可控制火车的大小布局。Rocrail 有客户端和服务器两种配置。客户端能够在 iDevices 或 Android 上运行。[Gerhard]的服务器运行在一个非常小的 Linux 计算机上，隐藏在布局下面。

他用了一个杨桃板而不是树莓派([Gehard]没能及时得到这个模型)，他用了一个杨桃板。Rocrail 服务器安装在该单板计算机上，并连接到 CAN 总线控制器。这是[Gehard]之前围绕 OpenWRT 构建的 [CAN/Ethernet gateway](http://lnxpps.de/can2udpe/openwrt/) 的一个进步，并使整个设备变得更小。

[Gehard]没有他的设计视频，但是休息之后你可以看到德国人有多喜欢他们在汉堡的模型火车。

[https://www.youtube.com/embed/ACkmg3Y64_s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ACkmg3Y64_s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)