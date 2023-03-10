# 用 Rickmote 控制器劫持 Chromecast

> 原文：<https://hackaday.com/2014/07/28/hijacking-cromecast-with-the-rickmote-controller/>

只需一个简单的 35 美元的加密狗，直接插入你的电视，就可以欣赏你最喜欢的电视节目、YouTube 频道和 Chromecast 提供的一切。作为一个支持 WiFi 的设备，也有可能劫持 Chromecast，迫使你的邻居看到[【里克·阿斯特利】说他永远不会放弃你](http://www.bishopfox.com/blog/2014/07/rickmote-controller-hacking-one-chromecast-time/)。

这个可怕的设备被称为 rickmote，它在树莓 Pi 上运行，并做了大量的 WiFi shennaigans 来劫持 Chromecast。首先，rickmote 范围内的所有无线网络都会被解除身份验证。当这种情况发生时，Chromecast 设备通常会抓狂，并试图自动重新配置自己，接受附近任何人的命令。rickmote 非常乐意为任何 Chromecast 设备提供这些命令，形式是 1987 年和 2008 年的热门歌曲。

下面是 rickmote 的视频演示，以及 ToorCon 描述劫持实际工作方式的讲话。

[https://www.youtube.com/embed/M7nqP8AvXUg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/M7nqP8AvXUg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/MZUYYgyUyh8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MZUYYgyUyh8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/BeyEGebJ1l4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BeyEGebJ1l4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)