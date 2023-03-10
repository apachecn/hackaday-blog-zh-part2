# HamRadioTweets 放出消息

> 原文：<https://hackaday.com/2014/12/23/hamradiotweets-gets-the-word-out/>

在危机时期，或者在政府极度控制的情况下，很难将关键信息传播给能提供帮助的人。一个很好的例子是 2011 年的阿拉伯之春。当你的网络连接被切断时，你会觉得好像一切都失去了。除非你有业余无线电。

对于许多人来说，一想到业余无线电就联想到老年人扭扭旋钮听静电的画面，但实际上它在我们的现代数字时代已经走过了漫长的道路。例如，你现在可以通过业余无线电发送推文。这个项目实际上是由[布鲁斯·萨瑟兰]在 2011 年开始的。在公民发布他们面临的极端暴力信息后，埃及政府关闭了该国的互联网接入。[Bruce]想找到一种方法来帮助其他人传播信息，于是他想出了[hamradioweets](http://hamradiotweets.com/ "HamRadioTweets")。这个系统允许用户通过业余无线电发送推文。

这个系统实际上是借用了一个叫做 APRS 的业余无线电服务。这项服务通常与 GPS 跟踪系统联系在一起，例如在近空间气球中发现的那些系统，但它也可以用于通过空中发送简单的文本消息。APRS 的成功要归功于遍布全球的接收站网络。这些电台可以接收信息，然后重新发送，大大扩展了原始发射机的覆盖范围。他们中的一些人甚至连上了互联网，通过传统方式将信息传送到非常困难和不可靠的地方。

[Bruce 的]系统连接到互联网组件，监视专门发送给“TWITR”的消息。基于 Python 的系统将读取这些消息，并通过 Twitter 转发。在 Twitter 更新了他们的 API 之后，这个项目就销声匿迹了。现在，它已经由[哈罗德·吉丁斯]在 Ruby 上重建。该项目网站被移交给[哈罗德]，他目前正在维护它。希望你永远都不需要使用这个软件，但是如果时间到了，你会很高兴它是可用的。在下面的视频中，你可以看到[Harold]将 APRS 的信息从国际空间站转发到推特上。

[https://www.youtube.com/embed/u_WWYBp1aJs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u_WWYBp1aJs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)