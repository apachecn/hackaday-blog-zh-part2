# 基于地理定位的欺骗 WiFi AP

> 原文：<https://hackaday.com/2013/08/27/spoofing-wifi-ap-based-geolocation/>

[Pierre Dandumont]刚刚完成了一个小项目，将使谷歌地图的定位功能物有所值。这是一种技术，[欺骗 WiFi 网络，以便重新定位通过 WiFi 网络报告的位置数据](http://www.journaldulapin.com/2013/08/26/dont-trust-geolocation/)。

他首先解释了现代设备获取位置数据的不同方式。GPS 是显而易见的，移动网络三角测量是众所周知的。但是使用 WiFi 网络对你来说可能是一个新的窍门。我们不能 100%确定，但我们认为谷歌能够根据 WiFi 接入点的已知 IP 地址查找位置数据(这将是一个很好的评论讨论)。要欺骗这个系统，你所要做的就是在谷歌地图试图锁定一个位置之前，将一些捕捉到的 AP 数据输入电脑。休息后的视频显示了合法地点的地图。在运行一个输出显示在地图上方的快速脚本后，位置被更改为欺骗位置。

[https://www.youtube.com/embed/ij-dWt7TU_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ij-dWt7TU_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)