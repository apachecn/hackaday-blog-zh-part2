# 使用 Android 作为网络服务器

> 原文：<https://hackaday.com/2012/06/21/using-an-android-as-a-webserver/>

![](img/412ac84b66384203ca6d2930faac92f7.png "android-webserver")

在 XDA 电视台的最新一集节目中，亚当·奥特勒将他的安卓手机变成了网络服务器。起初，这听起来可能很滑稽，但我们的手持设备不断增长的能力使它成为一个非常合理的选择。我们很难想出具体的用途，但我们确信从口袋里掏出手机提供一些内容是有价值的。

应用程序 [BotBrew Basil](https://play.google.com/store/apps/details?id=com.botbrew.basil) 使安装过程几乎自动化。它让你点击访问来安装[light tpd web server 包](http://www.lighttpd.net/)，并设置守护进程在引导时自动运行。就是这样！当然，您需要提供自己的 HTML 来提供服务。[Adam]为此使用了 HTML5 网站模板。

接下来，您还需要一种方法来解析电话的地址。在这种情况下，路由器会为其分配一个静态 IP，而动态 DNS 服务会提供一个映射到路由器位置的链接。但是由于这些手机运行的是 Linux(至少在最底层)，如果你想把“网络服务器”带在身边，添加一个 cron 任务将 IP 地址更新发送给服务应该是相当容易的。休息之后你可以看完整个视频。

具有讽刺意味的是，这是[亚当的]网络服务器的一次重大硬件升级。之前的版本是从[一个 Evalbot](http://hackaday.com/2010/10/23/evalbot-arrival-and-assembly/) 运行的。

[https://www.youtube.com/embed/Na7ssxlj_lo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Na7ssxlj_lo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)