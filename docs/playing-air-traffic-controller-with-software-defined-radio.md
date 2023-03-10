# 用软件无线电播放空中交通管制员

> 原文：<https://hackaday.com/2012/04/16/playing-air-traffic-controller-with-software-defined-radio/>

[![](img/16785fd14258139006bfc1966b9ae6a0.png "cockpit")](http://hackaday.com/wp-content/uploads/2012/04/cockpit.png)

成为一名空中交通管制员是一条非常酷的职业道路——你可以在电脑屏幕上看到飞机飞来飞去，像现代魔术师一样编排它们的飞行路线。[巴林特]送来了一台 DIY 航空制图仪,这样任何人都可以看到空中所有飞机的飞行路线，额外的好处是不会增加你心脏病发作或中风的风险。

[巴林特]的航空制图仪使用软件定义无线电覆盖雷达和来自飞机和控制塔的 [ACARS](http://en.wikipedia.org/wiki/Aircraft_Communications_Addressing_and_Reporting_System) 信息，这是在网络浏览器中运行的谷歌地球的一个实例。从软件定义的无线电获取所有无线电数据后，[巴林特]的服务器解析所有数据，并将其放入谷歌地球框架。在【巴林特】的[官方项目页面](http://spench.net/drupal/research/mode-s)上有大量关于硬件内部阴谋的信息、图片和解释。

目前，航空地图仅显示悉尼领空 500 公里以内的飞机，但[巴林特]正在其他飞机观察者的帮助下努力扩大覆盖范围。如果你愿意帮助(巴林特)扩大他的覆盖范围，一定要给他写信。

当然，【巴林特】是给我们那些便宜的 [USB 电视调谐器加密狗](http://hackaday.com/2012/03/20/software-defined-radio-from-a-usb-tv-capture-card/)一个[软件无线电源块](http://hackaday.com/2012/03/30/working-software-defined-radio-with-a-tv-tuner-card/)的家伙。就在几天前，我们看到这些加密狗[接收 GPS 数据](http://hackaday.com/2012/04/13/those-usb-tv-tuners-used-for-sdr-can-also-grab-gps-data/)，所以我们对这些小盒子在合适的人手里所能做的事情印象深刻。[巴林特]说他的航空制图应用程序可以和任何 GNU 无线电接收器一起工作，所以完全有可能用一些电视调谐器适配器来复制他的工作。

广告之后，有两段视频显示[巴林特]坐在悉尼机场附近的跑道尽头，看着抵达的飞机从他的头顶上方和他的笔记本电脑上飞来。这很酷，但我们会对纽约地区一个有进取心的黑客感兴趣，复制[巴林特]的作品。

[https://www.youtube.com/embed/bvg7WwzVldg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bvg7WwzVldg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/17_unMQyVWc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/17_unMQyVWc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)