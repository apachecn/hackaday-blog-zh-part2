# Forever.fm:无限节拍匹配的音乐

> 原文：<https://hackaday.com/2012/11/17/forever-fm-infinite-beat-matched-music/>

[![](img/1d29a8a986dfee12d2449504f7466a4a.png "Forever.fm")](http://hackaday.com/2012/11/17/forever-fm-infinite-beat-matched-music/foreverfm/)

[Forever.fm](http://forever.fm "Forever.fm") 是[ [彼得](http://petersobot.com/ "Peter Sobot") ]的[音云](http://soundcloud.com "SoundCloud")和[回声巢](http://the.echonest.com/ "The Echo Nest")的组合，播放连续的节拍匹配的音乐。结果就是一个网络电台一直在播放。

[Peter]提供了一篇很棒的[文章](http://petersobot.com/blog/introducing-forever-fm/ "Forever.fm Write Up")介绍他是如何开发这款应用的。服务器端是 Python，使用 [Tornado](http://www.tornadoweb.org/ "Tornado") web 服务器和 [Tornadio2](https://github.com/MrJoes/tornadio2 "Tornadio2") + [Socket。IO](http://socket.io/ "Socket.IO") 用于处理客户端的实时更新。为了应对流式音频的挑战，他为 Python 编写了一个蹩脚的接口，处理将原始的、节拍匹配的音频编码成 MP3 块。这些块被排队并由 web 服务器发送给客户机。

另一个挑战是选择歌曲。Forever.fm 从 SoundCloud 获取“最热门”的歌曲，并创建一个图表。然后，它找到遍历整个图的最短路径:一个[旅行推销员问题](http://en.wikipedia.org/wiki/Travelling_Salesman_Problem "Travelling Salesman Problem")。Forever.fm 使用的解决方案是找到一个迭代近似值，然后用它来制作一个曲目列表。当然，最终的音乐将会是 SoundCloud 上最热门的音乐。这可能符合，也可能不符合你的个人品味。

这里有很多不错的东西，如果你有兴趣查看细节，[Peter]在他的 github 上开源了代码。