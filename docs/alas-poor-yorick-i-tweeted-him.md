# 唉，可怜的约里克！我发微博给他了

> 原文：<https://hackaday.com/2013/10/19/alas-poor-yorick-i-tweeted-him/>

![yoreck the talking skull](img/efb5eb1c6815be6227783a4123e05928.png)

当阅读头骨的推特开始出现时，你知道万圣节就要到了。[马克]想把万圣节的精神带到他的工作场所，所以他建造了“约里克”。如果你担心的话，在这个黑客的创造中，没有人受到伤害(或被作为部分养殖)。Yorick 最初是一个解剖头骨模型，这种模型可能会在学校的生物实验室里找到。约里克的头骨为不是一个而是两个大脑提供了一个完美的外壳。

树莓派处理他的高级大脑功能。Pi 使用 Twitter API 来扫描@wedurick 的推文。一旦找到一条推文，它就会被发送到谷歌的翻译服务器。下一步是用谷歌翻译来执行文本到语音转换的一种众所周知的方法。程序很简单:派"http://translate.google.com/translate_tts 去？tl=en&q=hackaday "将返回该音频的 MP3 文件。要想有英国口音，只要换成 google.co.uk 口音就行了。

Pi 将音频传输到扬声器和 Arduino 的模拟输入引脚，Arduino 负责处理 Yorick 的低级大脑功能。Arduino 在一个紧密的循环中轮询音频。计算最后 3 个样本的平均值并将其映射到伺服位置。这导致了令人惊讶的逼真和自动的嘴部运动。我们认为这是黑客最好的部分。

马克独享自己的劳动成果是不公平的，所以约里克现在有了自己的直播频道。点击休息时间，听听 Yorick 对 Hack A Day 评论区的看法！我们提到过我们喜欢迎合吗？

[https://www.youtube.com/embed/pOmFqyIIQoo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pOmFqyIIQoo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)