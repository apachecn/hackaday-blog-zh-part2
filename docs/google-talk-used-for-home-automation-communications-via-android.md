# Google Talk 用于通过 Android 进行家庭自动化通信

> 原文：<https://hackaday.com/2013/01/07/google-talk-used-for-home-automation-communications-via-android/>

![home-automation-using-instant-messaging](img/a40967c654000a09d18cec25512f3fa7.png)

称[食肉动物的]家庭自动化项目令人印象深刻是一种保守的说法。他整合了一个快速、美观且易于使用的系统。为了与家中的物品互动，他使用了 X10 模块，这个例子只是简单地切换了一些台灯。但是底层的设置看起来非常完美，应该很容易扩展到任何用途。

上面链接的指南有所有的细节，但是最好的概述在休息后的视频中提供。【食肉动物】展示充当服务器的 Windows 8 机器。它连接了一个 am X10 收发器，以便与设备进行通信。他可以从上面看到的屏幕控制系统，但一切也可以从他的 Android 手机访问。两者之间的通信由即时通讯应用 Google Talk 处理，但命令是主屏幕快捷方式，不需要输入到 Google Talk 应用程序中。他修改了一个名为 TweetMyPC 的程序的源代码，使用 Google Talk API 在收到的信息中寻找关键词。与 SMS 或电子邮件相比，即时消息的延迟要低得多，因此命令的接收非常接近实时。反馈通过短信从服务器发送到手机。

[https://www.youtube.com/embed/HZxz26kGi-4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HZxz26kGi-4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)