# 对 Furby 进行逆向工程

> 原文：<https://hackaday.com/2013/01/28/reverse-engineering-the-furby/>

![Furby](img/ffcca63e26f178b9fab1748025373ca2.png)

Furby 拆卸是我们的最爱，没有什么比撕开一个令人毛骨悚然的会说话的变形电子猫头鹰/地狱野兽更好的了。你可以用一套螺丝刀和一把剪刀做很多事情，但需要一个真正聪明的人[在不拆卸的情况下逆向工程一个 Furby】(俄语，这里是](http://habrahabr.ru/post/166377/)[翻译](http://translate.google.com/translate?sl=ru&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&eotf=1&u=http%3A%2F%2Fhabrahabr.ru%2Fpost%2F166377%2F&act=url))。

新的 Furby 配备了一个 iOS 和 Android 应用程序，允许儿童通过喂它，给它命令，甚至将 furbi 翻译成英语来与 Furby 互动。这些应用程序的工作原理是播放一个 WAV 文件，该文件用命令编码，给 Furby 一些吃的东西，或者告诉它跳一支快乐的吉格舞。

这些 WAV 文件通过一个 4 位数、4 位代码连同校验和一起传送命令。Furby 实际上响应 10 位，这意味着 Furby 可能接受 1024 种不同的命令。

[iafan]编写了一个 Perl 脚本来监听 Android Furby 应用程序生成的音频，并将所有可能的命令与 Furby 采取的行动相关联。一切都在 git 上，允许任何人播放音频文件并控制 Furby 的情绪和行为。

有了这个，应该可以远程控制一只 Furby，让它在你收到电子邮件时跳舞，或者在有人转发你时让它生气。这比仅仅把一块毛皮放进碎木机要聪明得多，但是考虑到这些东西是多么令人毛骨悚然，我们不会说它更好。

# [](https://github.com/iafan)