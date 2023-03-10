# 使用 Codebender 远程上传到 Arduino

> 原文：<https://hackaday.com/2012/07/25/remote-uploading-to-an-arduino-with-codebender/>

[https://www.youtube.com/embed/KCHqhV6xPMg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KCHqhV6xPMg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

几周前，我们看到了 codebender，它是 Arduino IDE 的在线替代品，允许您从 web 浏览器将草图上传到您的板上。在 codebender 博客上[Vasilis]和他的团队正在推出一种通过以太网向 Arduino 远程上传代码的方法。现在你甚至不需要一个串行连接来编程一个 Arduino 它可以通过互联网传到隔壁房间或另一个大陆的黑板上。

这次黑客攻击的明星是 Ariadne bootloader，这是一个 TFTP 的实现，它允许任何支持以太网的 Arduino 通过互联网接收更新。Ariadne bootloader 仍然有一个小问题:通过以太网上传代码需要有人按下 Arduino 上的 reset 按钮，这完全否定了通过以太网编程 Arduino 的好处。

这个问题在早期的 Arduino 主板上已经解决了，所以我们确信[Vasilis]和他的团队能够在很短的时间内解决重置问题。如果你想看看远程 TFTP 引导程序，玩玩 codebender，你可以在 GitHub 上下载 Ariadne。