# 对 Android 的一次冒险让 VIC-20 说话了

> 原文：<https://hackaday.com/2015/02/13/an-adventure-into-android-makes-the-vic-20-speak/>

历史和[比尔·赫德]告诉我们，准将[乞求、借用或偷走了负责说&咒语](http://hackaday.com/2014/09/02/30-years-later-ted-finds-his-voice-a-commodore-story-part-i/)的工程师，为 C64 之后的几台计算机添加语音合成。这在实践中并不十分奏效，但是语音合成在很长一段时间内是 Commodore 场景的一部分。Votrax Type 'n Talk 是一个独立的语音合成器，插入 VIC-20 的扩展端口。它很贵，很稀有，但是有几个游戏支持它。[Jan]意识到语音合成技术在过去的 30 年里有了巨大的进步，并决定借助一部廉价的 Android 手机让[给他的 VIC 一个声音](http://jderogee.tripod.com/projects/BlueToothSpeechSynthesis/BlueToothSpeechSynthesis.html)。

一些 VIC-20 游戏，包括[Scott Adams] adventure games，通过扩展端口将音素作为文本发送，与 Votrax 语音合成器一起工作。从那里，Votrax 将负责将所有东西组装成可理解的东西，不需要在 VIC-20 上增加开销。[Jan]意识到由于 VIC 只是为每个音素吐出字符，他可以将这些单词重定向到一个更好、更现代的语音合成器。

一个小的蓝牙模块被连接到 VIC 上的用户端口，这个模块与一个便宜的 Android 智能手机配对。智能手机接收来自冒险游戏的串行流，并说出这些经典冒险游戏中所有场景的描述。

从视频来看，这是一种独特的体验，但同样的硬件和软件也可以添加到将在 VIC-20、C64 和 C128 上运行的任何程序中。下面视频。

[https://www.youtube.com/embed/8pPSYTCudCs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8pPSYTCudCs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)