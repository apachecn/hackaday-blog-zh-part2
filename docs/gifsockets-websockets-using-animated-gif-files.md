# Gifsockets:使用动画 GIF 文件的 WebSockets

> 原文：<https://hackaday.com/2013/02/07/gifsockets-websockets-using-animated-gif-files/>

![gifsockets](img/453c7e0ae91398412bcbdbafc9f6bda8.png)

使用动画 GIF 图像作为一个粗糙的网络接口是一个我们以前从未遇到过的想法，但它实际上很有意义。不是就它的整体效用而言，而是就动画文件以类似的方式工作这一事实而言。这些动画容器的性质是它工作的原因。GIF 不告诉浏览器预期有多少帧，所以连接保持打开，直到收到“嘿，这是最后一帧”命令。这可以用来将数据流式传输到任何可以播放动画的设备。

休息后的演示展示了这一点。Hello World 和一些其他测试消息被推送到浏览器，而不刷新页面。在我们看来，这才是有用的——无需刷新或任何底层客户端代码结构的实时更新。但是我们还没有研究细节，比如即使没有新的东西被发送，这也会消耗带宽吗？

当[Hans]写信告诉我们这个 gif 黑客时，他提到了 WebSockets 上的这个讨论区。我们还没有看完整个视频，但是显然有人把 gif 的把戏称为 90 年代的网络插座。

[https://player.vimeo.com/video/49447841](https://player.vimeo.com/video/49447841)