# 用 Pi 和 SDR 监视经过的飞机

> 原文：<https://hackaday.com/2014/11/27/keep-tabs-on-passing-jets-with-pi-and-sdr/>

显然，软件无线电非常酷。对于很多黑客来说，你只需要一个合适的项目就可以让你进入其中。提交给你批准的只是那个项目。西蒙·奥布里一直在用树莓 Pi 和 SDR 记录飞机从头顶飞过的视频。零部件便宜，大部分地方都有飞机经过；这可能是一个完美的项目。

我们不只是在谈论飞机穿过的静态框架，哦不。西蒙使用了两个业余爱好伺服系统和一些支架来平衡他的 Pi 相机板。DVB 加密狗允许钻机监听来自飞机的[自动相关监视广播](http://en.wikipedia.org/wiki/Automatic_dependent_surveillance-broadcast) (ADS-B)。该系统是大多数商用飞机的必备系统(实施的最后期限各不相同)。ADS-B 包括使用已知频率和协议从飞机上广播的定位数据。一旦[西蒙]锁定了这些数据，他就可以完成很多事情，比如让飞机保持在视频的中心，确定哪个航班正在被记录，以及自动上传镜头。有了这样一个令人惊叹的构建，我们肯定会看到更多的人尝试它。

[西蒙]写得也很好。他不仅包括一个 TL；博士，但钻了一个项目的总结和权利的坚韧不拔的细节。做得好的文档本身就值得庆祝！

[https://www.youtube.com/embed/qpSm0nYzry8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qpSm0nYzry8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)