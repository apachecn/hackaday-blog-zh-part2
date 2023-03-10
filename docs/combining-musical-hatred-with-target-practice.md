# 结合音乐仇恨和目标练习

> 原文：<https://hackaday.com/2015/07/16/combining-musical-hatred-with-target-practice/>

不是每个人都同意什么是好音乐，但在某些情况下，你会发现几乎每个人都同意什么是糟糕的。这是新泛大陆的人们在收听网络电台时发现的。当其中一首糟糕的歌曲击中他们的集体耳膜时，他们的愤怒就会增加，他们只需要跳过这首歌。

![This is how Engineers act if the song is super-awful](img/4e7ac6eee6e7dc059ec0f657c797ef28.png)

This is how Engineers act if the song is super-awful

他们没有使用 web 应用程序或简单的按钮来完成这个任务，而是将“跳过”按钮变成了一个 NERF 目标。他们称他们的发明为 [Boom Box Blaster](http://www.neo-pangea.com/news/of-note/dueling-for-musical-control.html) 并制作了一个关于它的精彩演示~~电影~~视频，在休息后可以找到。

灵感来自办公室里的一幅画，目标是一个小热气球。目标显然需要某种传感器，以便在被 NERF 飞镖击中时能够探测到。该小组尝试了几种不同类型的传感器，但最终选定了一种中型振动传感器。该传感器连接到 Arduino，然后 Arduino 通过串行连接与 Raspberry Pi 通信。Pi 使用 Python 脚本来监控 Arduino 的振动传感器。该系统还包括一些模拟火焰的橙色发光二极管和一个连接到绳子的伺服系统，绳子将气球悬挂在天花板上。每当记录到击中时，火焰就会亮起，气球就会升到空中，以表明击中了目标。

需要 Pi 来与集团选择的流媒体音乐服务对接；索诺斯。Sonos API 使得团队很容易将他们的目标与“跳过音轨”功能连接起来。他们只是编写了一个 Node.js 脚本，在 Pi 上运行，并在必要时发送适当的命令。现在每当收音机问这群人是否想堆雪人，他们都能响亮地回答:“不！”。他们只需要确保有足够的弹药。请务必查看[项目页面](http://www.neo-pangea.com/portfolio/neo-pangea/boombox-blaster.html)上的滑稽演示视频。

[https://www.youtube.com/embed/0NNIk0gHC6Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0NNIk0gHC6Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)