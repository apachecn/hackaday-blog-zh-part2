# Siri 使用 Ruby 控制 Arduino

> 原文：<https://hackaday.com/2013/02/01/siri-controlled-arduino-using-ruby/>

![siri-proxy-ruby-arduino](img/2dbec5c9b11ad78a80d7eaad7919f90d.png)

Hello World 代码的这个片段让[Nico Ritschel]使用 iPhones 内置的语音激活助手 Siri 来打开和关闭他的 Arduino 上的 Pin 13 LED。这里的诀窍是[使用 Ruby 编程语言让 Siri 代理通过 USB 连接与 Arduino](http://nicoritschel.com/Commanding-Arduino-with-Siri-via-Ruby.html) 对话。他称这个项目为 [siriproxy-arduino](https://github.com/nicoritschel/siriproxy-arduino) 。

黑客的一端是 SiriProxy，这是一个未经苹果批准的包，能够拦截发往苹果自己服务器的 Siri 消息。这些信息仍然被转发，但是每条信息都有一份副本供[尼科]自己使用。在事情的另一面，他在[Austinbv 的] [迪诺·杰姆](https://github.com/austinbv/dino)的工作上有所建树；一个便于控制 Arduino 的 Ruby 包。它包括一个上传到 Arduino 板上的草图，打开了一个 Ruby API。上面看到的代码集合定义了 LED 连接的 pin，然后监听特定的 Siri 命令来启动它。

休息后看看视频中[Nico]对模块的解释。

[https://www.youtube.com/embed/Ay1-9cJA8Nw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Ay1-9cJA8Nw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)